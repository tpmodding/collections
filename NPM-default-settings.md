Some Default settings for nginx Proxy Manager

add_header X-Xss-Protection "1; mode=block" always;
add_header X-Content-Type-Options "nosniff" always;
add_header X-Frame-Options "SAMEORIGIN" always;
proxy_hide_header X-Powered-By;
add_header 'Referrer-Policy' 'no-referrer';
add_header Permissions-Policy "accelerometer=();ambient-light-sensor=(); autoplay=();camera=();encrypted-media=();focus-without-user-activation=(); geolocation=();gyroscope=();magnetometer=();microphone=();midi=();payment=();picture-in-picture=(); speaker=();sync-xhr=();usb=();vr=()";
#CSP breaks some things, be careful
#add_header Content-Security-Policy "default-src 'self'; script-src 'self' 'unsafe-eval'; style-src 'self' 'unsafe-inline'; img-src 'self'; object-src 'none'";
