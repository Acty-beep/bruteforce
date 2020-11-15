import pyautogui
import random

chars = "abcdefghijklmnopqrstuvwxyz"
char_list = list(chars)

real_pwd = pyautogui.password('Enter password: ')

guess_pwd = ""

while guess_pwd != real_pwd:
	guess_pwd = random.choices(char_list, k=len(real_pwd))
	print("Denied: ", str(guess_pwd))

	if guess_pwd == list(real_pwd):
		print("\nAccess Granted: ~ ", "".join(guess_pwd))
		break
