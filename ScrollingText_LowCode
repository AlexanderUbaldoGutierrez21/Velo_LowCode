import { timeline } from 'wix-animations';
import wixWindow from 'wix-window';

function getWindowSize() {
    return wixWindow.getBoundingRect()
    .then((windowSize) => {
        return windowSize.window;
    });
}

$w.onReady(function () {

    let scrollLtR = $w('#scrollLRt');
    let scrollingLtR = timeline({ repeat: -1});

    getWindowSize()
    .then((windowSize) => {

       scrollingLtR
        .add(scrollLtR, {
            duration: 10000,
            x: -windowSize.width,
            easing: 'easeLinear'
        });
    scrollingLtR.play();
    
    });
});