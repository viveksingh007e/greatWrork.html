<center>
    <button onclick="startEyeExercise()" style="height:100px;width:200px">
        EyeExercise
    </button>
    <br>
</center>

<script src="https://unpkg.com/nosleep.js@0.12.0/dist/NoSleep.min.js"> 
function speakAndWait(text, waitSeconds) {
    speechSynthesis.speak(new SpeechSynthesisUtterance(text));
    return new Promise(resolve => 
        setTimeout(resolve, waitSeconds * 1000)
    );
}

async function startEyeExercise() {
    await noSleep.enable();
    await speakAndWait('Welcome back dear! Great that you came up with this idea. We will start eyes exercise now. This will last just 11 minutes', 1);
    await speakAndWait('Start with rolling your eyes gently for 2 minute. Starting now!', 60);
    await speakAndWait('Great! Relax now', 5);
    await speakAndWait('Roll for another 1 minute', 60);
    await speakAndWait('Great! Relax now', 5);

    await speakAndWait('Now, Gently massage your eyes sockets for 2 minute. Starting now!', 60);
    await speakAndWait('Great! Relax now', 5);
    await speakAndWait('Massage for another 1 minute', 60);
    await speakAndWait('Great! Relax now', 5);

    await speakAndWait('Now, pin your acupressure points for 3 minutes. Starting now!', 60);
    await speakAndWait('Great! Relax now', 5);
    await speakAndWait('pin for 2 minutes', 60);
    await speakAndWait('Great! Relax now', 5);
    await speakAndWait('pin for another 1 minute', 60);
    await speakAndWait('Great! Relax now', 5);

    await speakAndWait('Awesome So far! Now focus adjustment for near and far points for 4 minutes', 60);
    await speakAndWait('Great! Relax now', 5);
    await speakAndWait('focus for another 3 minutes', 60);
    await speakAndWait('Great! Relax now', 5);
    await speakAndWait('focus for another 2 minutes', 60);
    await speakAndWait('Great! Relax now', 5);
    await speakAndWait('focus for last 1 minute', 60);

    await speakAndWait('Terrific Work! we have completed today\'s exercise', 0);
    noSleep.disable();
}
</script>
