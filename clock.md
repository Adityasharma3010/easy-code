```css
        #clock {
            font-size: 16px;
			font-weight:500;
			line-height: 19.36px;
            color: #fff;
        }
```
```html
   <div id="clock">00:00:00</div>
```
```js
        function updateClock() {
            const now = new Date();
            const hours = String(now.getHours()).padStart(2, '0');
            const minutes = String(now.getMinutes()).padStart(2, '0');
            const seconds = String(now.getSeconds()).padStart(2, '0');
            const timeString = `${hours}:${minutes}:${seconds}`;
            document.getElementById('clock').textContent = "(GMT+8:00) "+timeString;
        }

        setInterval(updateClock, 1000);
        updateClock(); 
```
