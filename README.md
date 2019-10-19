# auto-whatsapp
Programmatically send WhatsApp messages

To get Started:

Install Python and Mozila Firefox

1. Clone The Repo
2. Change the config.py file in main directory 
  i. binary_location - change the binary location & point it to firefox.exe in your local system
  ii. Download Geckodriver and point gecckodriver.exe to fire_fox_driver_path
      Dowload it from https://github.com/mozilla/geckodriver/releases
  iii. fire_fox_profile_path - open mozila firefox and once login to your whatsapp, then open settings and copy the profiles path.
  

after all these steps, go to main directory and run pip install -r requirements.txt

once all the dependencies gets downloaded,

go to main.py and change the contact name and message name in line print(client_headless.send_message('ME', 'Testing', Constants.TEXT))

Note that contact name should be exactly same as the contact name in your whatsapp contact, For example, your contact name is John and the text you want to send is Hi John, you can change the line as:
print(client_headless.send_message('John', 'Hi John', Constants.TEXT))

after this change, execute the command python main.py

once everything gets loaded and executed, True gets returned to the console, that means the message has been sent.
