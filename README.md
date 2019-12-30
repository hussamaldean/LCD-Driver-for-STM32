# LCD-Driver-for-STM32
HD44780 library for Stm32 using hal library


Features:

4bit

String printing

Number printing

Set cursor position

Clear screen

Example

>Lcd_PortType ports[] = {D4_GPIO_Port, D5_GPIO_Port, D6_GPIO_Port, D7_GPIO_Port};

 Lcd_PinType pins[] = {D4_Pin, D5_Pin, D6_Pin, D7_Pin};
 
 Lcd_HandleTypeDef lcd = Lcd_create(ports, pins, RS_GPIO_Port, RS_Pin, EN_GPIO_Port, EN_Pin, LCD_4_BIT_MODE);
 
 Lcd_cursor(&lcd, 0,0);
 
 Lcd_string(&lcd, "Hussam - STM32");
 
 
Remember to include lcd.h in your code after the main ;) 
