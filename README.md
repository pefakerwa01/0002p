const words = ["Live Stream", "Overlay Design", "Custom Effects", "Smooth Animations", "Professional Look"];
const topLeftElement = document.getElementById("top-left");

let wordIndex = 0;

function updateTopLeftText() {
    topLeftElement.innerText = words[wordIndex];
    wordIndex = (wordIndex + 1) % words.length;
}

setInterval(updateTopLeftText, 120000); // Updates every 2 minutes

// Ensure initial display
updateTopLeftText();
