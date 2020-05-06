# MistySkillSelector

*This example was last tested on `robotVersion 1.16.1.10505`*

This skill lets you use Misty's capacitive touch and bump sensors to view, start, and stop Misty's skills. When it runs:

* Touch Misty's chin to toggle the display layers that show the installed skills and their current run status.
* Touch Misty's front left and right bump sensors to "scroll" through the list of skills.
* Touch Misty's rear left or right bump sensor to start or stop the selected skill.

This skills uses the [`misty.RegisterEvent()`](https://docs.mistyrobotics.com/misty-ii/javascript-sdk/api-reference/#misty-registerevent) method to register for [`TouchSensor`](https://docs.mistyrobotics.com/misty-ii/robot/sensor-data/#touchsensor) and [`BumpSensor`](https://docs.mistyrobotics.com/misty-ii/robot/sensor-data/#bumpsensor) event messages. It uses the [`misty.DisplayText()`](https://docs.mistyrobotics.com/misty-ii/javascript-sdk/api-reference/#misty-displaytext) and [`misty.SetTextDisplaySettings()`](https://docs.mistyrobotics.com/misty-ii/javascript-sdk/api-reference/#misty-settextdisplaysettings) to update Misty's [display layers](https://docs.mistyrobotics.com/misty-ii/robot/misty-ii/#using-misty-39-s-display) in response to the user's actions. 

You can run this code on your robot by uploading the files from this folder to Misty via the Skill Runner web tool. Alternately, refer to this code sample (or copy and paste it into your own skills) when working on similar functionality.

---

**WARRANTY DISCLAIMER.**

* General. TO THE MAXIMUM EXTENT PERMITTED BY APPLICABLE LAW, MISTY ROBOTICS PROVIDES THIS SAMPLE SOFTWARE “AS-IS” AND DISCLAIMS ALL WARRANTIES AND CONDITIONS, WHETHER EXPRESS, IMPLIED, OR STATUTORY, INCLUDING THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE, TITLE, QUIET ENJOYMENT, ACCURACY, AND NON-INFRINGEMENT OF THIRD-PARTY RIGHTS. MISTY ROBOTICS DOES NOT GUARANTEE ANY SPECIFIC RESULTS FROM THE USE OF THIS SAMPLE SOFTWARE. MISTY ROBOTICS MAKES NO WARRANTY THAT THIS SAMPLE SOFTWARE WILL BE UNINTERRUPTED, FREE OF VIRUSES OR OTHER HARMFUL CODE, TIMELY, SECURE, OR ERROR-FREE.
* Use at Your Own Risk. YOU USE THIS SAMPLE SOFTWARE AND THE PRODUCT AT YOUR OWN DISCRETION AND RISK. YOU WILL BE SOLELY RESPONSIBLE FOR (AND MISTY ROBOTICS DISCLAIMS) ANY AND ALL LOSS, LIABILITY, OR DAMAGES, INCLUDING TO ANY HOME, PERSONAL ITEMS, PRODUCT, OTHER PERIPHERALS CONNECTED TO THE PRODUCT, COMPUTER, AND MOBILE DEVICE, RESULTING FROM YOUR USE OF THIS SAMPLE SOFTWARE OR PRODUCT.

Please refer to the Misty Robotics End User License Agreement for further information and full details: https://www.mistyrobotics.com/legal/end-user-license-agreement/

--- 

*Copyright 2020 Misty Robotics*<br>
*Licensed under the Apache License, Version 2.0*<br>
*http://www.apache.org/licenses/LICENSE-2.0*