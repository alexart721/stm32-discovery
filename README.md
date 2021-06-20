# stm32-discovery
Discovery projects for the STM32F407 discovery board

blinking-lights

- First project! Made lights blink...

blinking-lights-button

- Blinking light frequency responds to user button push, switching between 500ms delay, 100ms delay, and random from 50ms up to 1.5 second delay between light toggle

- Have to set pinout PA0 to GPIO_EXTI0, and then under NVIC check EXTI line0 interrupt, then edit code in stm32f4xx_it.c as shown, importing external variable tDelay from main.c