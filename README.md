<html>
<body style="background:DarkOliveGreen; color: white; text-align: center; padding: 50px 20px; font-family: Arial;">
<center>
    <button onclick="startEyeExercise()" style="height:90px;width:120px;background:OliveDrab;border-radius:30px">
        <b style="font-size:60px;">🧐</b>
    </button>
    <br><font color=gold><b>13 min</b></font><br><br>
	 <button onclick="startBellyExercise()" style="height:90px;width:120px;background:OliveDrab;border-radius:30px">
        <b style="font-size:60px;">🦘</b>
    </button>
    <br><font color=gold><b>8 min</b></font><br><br>
	<button onclick="startYog()" style="height:90px;width:120px;background:OliveDrab;border-radius:30px">
        <b style="font-size:60px;">🧘</b>
    </button>
    <br><font color=gold><b>9 min</b></font><br><br>
	<button onclick="startRun()" style="height:90px;width:120px;background:OliveDrab;border-radius:30px">
        <b style="font-size:60px;">🏃</b>
    </button>
    <br><font color=gold><b>5 min</b></font><br><br>
</center>

<script src="https://unpkg.com/nosleep.js@0.12.0/dist/NoSleep.min.js"></script>
<script>
// Initialize NoSleep
const noSleep = new NoSleep();

function speakAndWait(text, waitSeconds) {
    speechSynthesis.speak(new SpeechSynthesisUtterance(text));
    return new Promise(resolve => 
        setTimeout(resolve, waitSeconds * 1000)
    );
}

async function startEyeExercise() {
    try {
        // Enable no sleep - requires user gesture
        await noSleep.enable();
        console.log('NoSleep enabled');
        
        await speakAndWait('Welcome back dear! Great that you came up with this idea. We will start eyes exercise now. This will last just 13 minutes. Sit comfortably and get in position', 25);
        await speakAndWait('We will start with rolling the eyes gently for 4 minutes. Start by rolling side ways for 1 minute', 75);
        await speakAndWait('Great! Relax now', 10);
        await speakAndWait('Now, Roll eyes up and down for a minute', 70);
        await speakAndWait('Great! Relax now', 10);
		await speakAndWait('Now, Roll eyes clockwise for a minute', 70);
        await speakAndWait('Great! Relax now', 10);
		await speakAndWait('Now, Roll eyes anti-clockwise for a minute', 70);
        await speakAndWait('Perfect! The rolling is complete now. Relax!', 15);

        await speakAndWait('Now, Gently massage your eyes sockets for 2 minute.', 70);
        await speakAndWait('Continue for last 1 minute', 70);
        await speakAndWait('Perfect! The massage is complete now. Relax!', 15);

        await speakAndWait('Now, pin your acupressure points for 3 minutes', 70);
        await speakAndWait('Continue for another 2 minutes', 70);
        await speakAndWait('Just 1 minute remaining now', 70);
        await speakAndWait('Perfect! The acupressure is complete now. Relax!', 15);

        await speakAndWait('Awesome So far! Now focus adjustment for near and far points for 4 minutes. Starting now!', 70);
        await speakAndWait('Great! Relax now', 10);
        await speakAndWait('continue for another 3 minutes', 70);
        await speakAndWait('Great! Relax now', 10);
        await speakAndWait('continue for another 2 minutes', 70);
        await speakAndWait('Great! Relax now', 10);
        await speakAndWait('just 1 minute remaining now', 70);

        await speakAndWait('Terrific Work! we have completed all eye exercises. See you again!', 0);
        
    } catch (error) {
        console.error('Error:', error);
        alert('Error starting exercise: ' + error.message);
    } finally {
        // Always disable no sleep when done
        noSleep.disable();
        console.log('NoSleep disabled');
    }
}

async function startBellyExercise() {
    try {
        // Enable no sleep - requires user gesture
        await noSleep.enable();
        console.log('NoSleep enabled');
        
        await speakAndWait('Welcome dear! We will start belly exercise now. This will last just 8 minutes. Take your time to get in position. We will start in 10 seconds', 20);
        
		await speakAndWait('Are you ready now!', 5);
		await speakAndWait('Lets start jumping for 2 minutes straight. Starting now!', 130);
        await speakAndWait('Great! Relax now for 20 seconds', 30);
      
        await speakAndWait('Lets start jumping for another 2 minutes. This is second set. Starting now!', 130);
		await speakAndWait('Great! Relax now for 20 seconds', 30);
		
		await speakAndWait('Lets start jumping for another 2 minutes. This is third set. Starting now!', 130);
		await speakAndWait('Great! Relax now for 20 seconds', 30);
		
		await speakAndWait('Lets start jumping for another 2 minutes. This is last set. Starting now!', 130);
		
        await speakAndWait('Terrific Work! we have completed jumping exercise. See you again!', 0);
        
    } catch (error) {
        console.error('Error:', error);
        alert('Error starting exercise: ' + error.message);
    } finally {
        // Always disable no sleep when done
        noSleep.disable();
        console.log('NoSleep disabled');
    }
}

async function startYog() {
    try {
        // Enable no sleep - requires user gesture
        await noSleep.enable();
        console.log('NoSleep enabled');
        
        await speakAndWait('Welcome dear! We will start Yoga now. This will last just 8 minutes. Take your time to get in position. We will start in 10 seconds', 20);
		
		await speakAndWait('Lets start head shine for 5 minutes. Starting now!', 70);
        await speakAndWait('Another 4 minutes remaining', 70);
		await speakAndWait('Great! Relax now for 10 seconds', 12);
		await speakAndWait('Continue for another 3 minutes', 70);
		await speakAndWait('Just 2 minute remaining now!', 70);
		await speakAndWait('Great! Relax now for 10 seconds', 12);
		await speakAndWait('Last 1 minute remaining now!', 70);
		await speakAndWait('Perfect! head shine is complete now. Relax!', 20);
		
		await speakAndWait('Lets start Nose breathing for 2 minutes. Starting now!', 70);
		await speakAndWait('just 1 minute remaining now', 70);
		await speakAndWait('Perfect! Nose breathing is complete now. Relax!', 20);
		
        await speakAndWait('Lets rub nails for 2 minutes. Starting now!', 70);
		await speakAndWait('just 1 minute remaining now', 70);		
		
		await speakAndWait('Terrific Work! we have completed Yoga. See you again!', 0);
        
    } catch (error) {
        console.error('Error:', error);
        alert('Error starting exercise: ' + error.message);
    } finally {
        // Always disable no sleep when done
        noSleep.disable();
        console.log('NoSleep disabled');
    }
}
async function startRun() {
    try {
        // Enable no sleep - requires user gesture
        await noSleep.enable();
        console.log('NoSleep enabled');
        
        await speakAndWait('Welcome dear! We will start Running now. This will last just 5 minutes. Take your time to get in position. We will start in 15 seconds', 25);
		
		await speakAndWait('Lets hit the road now! Run!', 65);
        await speakAndWait('Another 4 minutes remaining', 65);
		await speakAndWait('Continue for another 3 minutes', 65);
		await speakAndWait('Just 2 minute remaining now!', 65);
		await speakAndWait('Great running! Last 1 minute remaining now!', 65);
		
		await speakAndWait('Terrific! Perfect! Run is complete now. Relax! See you again!', 0);
        
    } catch (error) {
        console.error('Error:', error);
        alert('Error starting exercise: ' + error.message);
    } finally {
        // Always disable no sleep when done
        noSleep.disable();
        console.log('NoSleep disabled');
    }
}
</script>

</body>
</html>
