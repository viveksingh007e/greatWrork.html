<Center><button onclick="
    function speakAndWait(text, waitSeconds) {
        speechSynthesis.speak(new SpeechSynthesisUtterance(text));
        return new Promise(resolve => 
            setTimeout(resolve, waitSeconds * 1000)
        );
    }

async function startExercise() {
await speakAndWait('Welcome Back! Great that you came up with this idea. We will start eyes exercise now. This will last just 10 minutes', 1);
await speakAndWait('Start with rolling your eyes gently for 2 minute. Starting now!', 60);
await speakAndWait('another 1 minute', 60);
await speakAndWait('Great! Relax now', 5);

await speakAndWait('Now, Gently massage your eyes sockets for 2 minute', 60);
await speakAndWait('Great! Relax now', 5);
await speakAndWait('Another 1 minute', 60);
await speakAndWait('Great! Relax now', 5);

await speakAndWait('Now pin your acupressure points for 3 minutes', 60);
await speakAndWait('Another 2 minute', 60);
await speakAndWait('Great! Relax now', 5);
await speakAndWait('Another 1 minute', 60);
await speakAndWait('Great! Relax now', 5);

await speakAndWait('Great So far! Now focus adjustment for near and far for 4 minutes', 60);
await speakAndWait('Great! Relax now', 5);
await speakAndWait('Another 3 minutes', 60);
await speakAndWait('Great! Relax now', 5);
await speakAndWait('Another 2 minutes', 60);
await speakAndWait('Great! Relax now', 5);
await speakAndWait('Last 1 minute', 60);
await speakAndWait('Great! Relax now', 5);

await speakAndWait('Great Work! we have completed today\'s exercise', 0);
    }
    
    startExercise();
" style="height:100px;width:200px">EyeExercise</button></center>
