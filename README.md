# android-notification
from kivy.app import App
from kivy.uix.button import Button
import plyer

class whatsapp(App):
    def build(self):
        return Button(text='Whatsapp', on_press=self.notify)

    def notify(self, obj):
        plyer.notification.notify(title="techsnap", messsage="welcome")

whatsapp().run()
