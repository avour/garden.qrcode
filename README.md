Module QRCode
=============


A QRCode Widget.


Usage::

 Python::

    from kivy.garden.qrcode import QRCodeWidget
    parent.add_widget(QRCodeWidget(range=(0, 100)))

 kv::

    BoxLayout:
        orientation: 'vertical'
        Button:
            text: 'press to change qrcode'
            on_release: qr.data = "Kivy Rocks!"
        QRCodeWidget:
            id: qr
            data: 'Hello World'
