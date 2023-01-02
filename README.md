# QR-CODE-PROJECT
I made a QR-CODE  to access the insta-gram profile
import qrcode
from PIL import Image
QR=qrcode.QRCode(version=1,
                 error_correction=qrcode.constants.ERROR_CORRECT_H,
                 box_size=15,border=5,)
QR.add_data("https://www.instagram.com/p___for__pramod/")
QR.make(fit=True)
img=QR.make_image(fill_color="red",back_color="GREEN")
img.save("insta_profile.png")
