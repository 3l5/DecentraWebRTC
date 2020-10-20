# DecentraWebRTC
Installation


npm install

Building


npm run build


Local Server


npm start


Testing


npm test


Starting App
‎
‎
‎‎
‎
‎
‎
‎
‎
‎

Peer starting collaboration has to generate a uuid using


var grtcID = GRTC.uuid(); // static function


After that pass that to GRTC module






window.history.pushState('', '', '#' + grtcID); // optional to add to url so can share with others.
var grtc = new GRTC(grtcID, window.location.origin,  true); // 3rd param is transport layer for encrypted session.

Peer not starting collaboration has to join and get that grtcID somehow possibly by sharing url
