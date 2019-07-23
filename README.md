# readme

Page URL: https://sequoiagizmo.github.io/hohwtour/

To launch tour:
1. Press the three circles in upper right hand corner
2. Press "Fullscreen"

const _toggleFullScreen = function _toggleFullScreen() {
    if (document.fullscreenElement || document.mozFullScreenElement || document.webkitFullscreenElement) {
        if (document.cancelFullScreen) {
            document.cancelFullScreen();
        } else {
            if (document.mozCancelFullScreen) {
                document.mozCancelFullScreen();
            } else {
                if (document.webkitCancelFullScreen) {
                    document.webkitCancelFullScreen();
                }
            }
        }
    } else {
        const _element = document.documentElement;
        if (_element.requestFullscreen) {
            _element.requestFullscreen();
        } else {
            if (_element.mozRequestFullScreen) {
                _element.mozRequestFullScreen();
            } else {
                if (_element.webkitRequestFullscreen) {
                    _element.webkitRequestFullscreen(Element.ALLOW_KEYBOARD_INPUT);
                }
            }
        }
    }
};

<iframe width='960' height='540' src='https://roundme.com/embed/Al01f0H5m7KrWug3lgfB' frameborder='0' webkitallowfullscreen mozallowfullscreen allowfullscreen></iframe>

