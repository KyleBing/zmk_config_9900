# BB9900 wireless Keyboard: zmk-config

| key          | 含义            | 说明                                                                                                                                                   |
|--------------|---------------|------------------------------------------------------------------------------------------------------------------------------------------------------|
| &kp	         | 普通按键          | 	点击的时候发送指定按键                                                                                                                                         |
| &mt	         | 普通按键 + 长按	    | 长按的时候发送一个键，点击的时候发送另一个键                                                                                                                               |              
| &kt	         | toggle 按键	    | 按键状态切换，点击时将指定键处于按下的状态，直到这个键被再次点击                                                                                                                     | 
| &sk	         | 粘滞按键	         | 点击后该键将处于按下的状态，直到点击其它按键，该键才恢复弹起状态                                                                                                                     |                                                                                                                                                                                                                                                   |
| &gresc	      | Grave Escape	 | Sends Grave Accent ` keycode if shift or GUI is held, sends Escape keycode otherwise                                                                 |                                                                                                                                                                                                                                                   |
| &caps_word	  | Caps Word	    | Behaves similar to caps lock, but automatically deactivates when any key not in a continue list is pressed, or if the caps word key is pressed again |                                                                                                                                                                                                                                                   |
| &key_repeat	 | Key Repeat	   | Sends again whatever keycode was last sent                                                                                                           |                                                                                                                                                                                                                                                   |

Hey 👋 welcome. Use this repo to generate your own ZMK keymap for the BB9900 BLE keyboard.  
> [ZMK 固件中可以使用哪些按键](https://zmk.dev/docs/codes)  
> [ZMK 固件可以使用哪些动作](https://zmk.dev/docs/behaviors)  

## 如何构建自己的键盘键位
1. 注册一个 github 账号
2. Fork 这个仓库。 ![fork](https://github.com/ZitaoTech/zmk-config_9900/assets/145678024/4ffc71b9-0ed3-4ae9-ace7-99078dd1d9bc)  
3. 编辑键位文件 `config/bb9900.keymap`，参照 [ZMK 固件中可以使用哪些按键](https://zmk.dev/docs/codes)  。![image](https://github.com/ZitaoTech/zmk-config_9900/assets/145678024/a0900a5c-6650-4794-9d11-a17c380a973d)  
4. 编辑完键位文件之后，提交你的修改 ![image](https://github.com/ZitaoTech/zmk-config_9900/assets/145678024/c708dbd0-6c90-49da-aeda-053668ae43c8)
 查看 github 中 Action 标签页，没有错误的话会生成一个 firmware 的文件 ![image](https://github.com/ZitaoTech/zmk-config_9900/assets/145678024/fb534054-add6-4517-8643-8270cbf6d8c7)
 下载它即可。![image](https://github.com/ZitaoTech/zmk-config_9900/assets/145678024/ae6a1646-c8ab-4966-b969-12e68ecaa0ab)
![image](https://github.com/ZitaoTech/zmk-config_9900/assets/145678024/a6140108-9e27-4d51-aa42-ba12233b8738)
5. 解决下载后的文件，会解压出一个名为 `bb9900-zmk.uf2` 的文件，这个就是键盘的固件文件。  
6. 将这个固件拖放到键盘的盘符中即可完成更新，具体查看键盘说明书：[如何更新固件](https://github.com/ZitaoTech/BB9900-USB_BLE_Keyboard?tab=readme-ov-file#-how-to-update-the-firmware---) 
