# onesignal-Subscription-Bell

##### LINK CDN
```javascript
<script src="https://cdn.onesignal.com/sdks/OneSignalSDK.js" async=""></script>
```

##### Script
```javascript
<script>
    window.OneSignal = window.OneSignal || [];
    OneSignal.push(function() {
        OneSignal.init({
            appId: "{You APP ID}",
            notifyButton: {
                enable: true,
                colors: { // Customize the colors of the main button and dialog popup button
                'circle.background': '#ff3ff9',
                'circle.foreground': '#fff',
                'badge.background': '#ff3ff9',
                'badge.foreground': '#fff',
                'badge.bordercolor': '#fff',
                'pulse.color': '#fff',
                'dialog.button.background.hovering': '#ff9ff3',
                'dialog.button.background.active': '#ff9ff3',
                'dialog.button.background': '#ff3ff9',
                'dialog.button.foreground': '#fff'
                },
                text: {
                    'tip.state.unsubscribed': 'สมัครรับการแจ้งเตือน',
                    'tip.state.subscribed': "คุณสมัครรับการแจ้งเตือน",
                    'tip.state.blocked': "คุณได้ปิดกั้นการแจ้งเตือน",
                    'message.prenotify': 'คลิกเพื่อสมัครรับการแจ้งเตือน',
                    'message.action.subscribed': "ขอบคุณสำหรับการสมัคร!",
                    'message.action.resubscribed': "คุณสมัครรับการแจ้งเตือน",
                    'message.action.unsubscribed': "คุณจะไม่ได้รับการแจ้งเตือนอีก",
                    'dialog.main.title': 'จัดการการแจ้งเตือนของเว็บไซต์',
                    'dialog.main.button.subscribe': 'ติดตาม',
                    'dialog.main.button.unsubscribe': 'ยกเลิกการเป็นสมาชิก',
                    'dialog.blocked.title': 'เลิกบล็อกการแจ้งเตือน',
                    'dialog.blocked.message': "ทำตามคำแนะนำเหล่านี้เพื่ออนุญาตการแจ้งเตือน:"
                },
            },
            // Other init Options
            welcomeNotification: {
                "title": "You Title",
                "message": "Thanks for subscribing!",
                // "url": "" /* Leave commented for the notification to not open a window on Chrome and Firefox (on Safari, it opens to your webpage) */
            },
        });
    });
```

###### ตั่งค่าสี
```javascript
colors: { // Customize the colors of the main button and dialog popup button
         'circle.background': '#ff3ff9',
         'circle.foreground': '#fff',
         'badge.background': '#ff3ff9',
         'badge.foreground': '#fff',
         'badge.bordercolor': '#fff',
         'pulse.color': '#fff',
         'dialog.button.background.hovering': '#ff9ff3',
         'dialog.button.background.active': '#ff9ff3',
         'dialog.button.background': '#ff3ff9',
         'dialog.button.foreground': '#fff'
}
```

###### ตั่งค่าข้อความ
```javascript
text: {
       'tip.state.unsubscribed': 'สมัครรับการแจ้งเตือน',
       'tip.state.subscribed': "คุณสมัครรับการแจ้งเตือน",
       'tip.state.blocked': "คุณได้ปิดกั้นการแจ้งเตือน",
       'message.prenotify': 'คลิกเพื่อสมัครรับการแจ้งเตือน',
       'message.action.subscribed': "ขอบคุณสำหรับการสมัคร!",
       'message.action.resubscribed': "คุณสมัครรับการแจ้งเตือน",
       'message.action.unsubscribed': "คุณจะไม่ได้รับการแจ้งเตือนอีก",
       'dialog.main.title': 'จัดการการแจ้งเตือนของเว็บไซต์',
       'dialog.main.button.subscribe': 'ติดตาม',
       'dialog.main.button.unsubscribe': 'ยกเลิกการเป็นสมาชิก',
       'dialog.blocked.title': 'เลิกบล็อกการแจ้งเตือน',
       'dialog.blocked.message': "ทำตามคำแนะนำเหล่านี้เพื่ออนุญาตการแจ้งเตือน:"
}
```

###### ข้อความสำหรับคนกดติดตาม
```javascript
welcomeNotification: {
     "title": "ขอบคุณ",
     "message": "ขอบคุณสำหรับการติดตาม!",
     "url": "https://www.animejapanth.com" /* Leave commented for the notification to not open a window on Chrome and Firefox (on Safari, it opens to your webpage) */
}
```
