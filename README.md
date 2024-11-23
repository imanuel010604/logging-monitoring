membuat 2 instance ec2 deploy nginx, grafana, prometheus dan instance satuya menginstal K6 untuk teaster
contoh teaster :

         /\      Grafana   /‾‾/  
    /\  /  \     |\  __   /  /   
   /  \/    \    | |/ /  /   ‾‾\ 
  /          \   |   (  |  (‾)  |
 / __________ \  |_|\_\  \_____/ 

     execution: local
        script: load-test.js
        output: -

     scenarios: (100.00%) 1 scenario, 1 max VUs, 10m30s max duration (incl. graceful stop):
              * default: 1 iterations for each of 1 VUs (maxDuration: 10m0s, gracefulStop: 30s)


     ✓ status is 200

     checks.........................: 100.00% 1 out of 1
     data_received..................: 1.4 kB  591 kB/s
     data_sent......................: 80 B    34 kB/s
     http_req_blocked...............: avg=992.88µs min=992.88µs med=992.88µs max=992.88µs p(90)=992.88µs p(95)=992.88µs
     http_req_connecting............: avg=941.26µs min=941.26µs med=941.26µs max=941.26µs p(90)=941.26µs p(95)=941.26µs
     http_req_duration..............: avg=1.04ms   min=1.04ms   med=1.04ms   max=1.04ms   p(90)=1.04ms   p(95)=1.04ms  
       { expected_response:true }...: avg=1.04ms   min=1.04ms   med=1.04ms   max=1.04ms   p(90)=1.04ms   p(95)=1.04ms  
     http_req_failed................: 0.00%   0 out of 1
     http_req_receiving.............: avg=63.88µs  min=63.88µs  med=63.88µs  max=63.88µs  p(90)=63.88µs  p(95)=63.88µs 
     http_req_sending...............: avg=51.45µs  min=51.45µs  med=51.45µs  max=51.45µs  p(90)=51.45µs  p(95)=51.45µs 
     http_req_tls_handshaking.......: avg=0s       min=0s       med=0s       max=0s       p(90)=0s       p(95)=0s      
     http_req_waiting...............: avg=934.11µs min=934.11µs med=934.11µs max=934.11µs p(90)=934.11µs p(95)=934.11µs
     http_reqs......................: 1       422.417172/s
     iteration_duration.............: avg=2.29ms   min=2.29ms   med=2.29ms   max=2.29ms   p(90)=2.29ms   p(95)=2.29ms  
     iterations.....................: 1       422.417172/s


running (00m00.0s), 0/1 VUs, 1 complete and 0 interrupted iterations
default ✓ [======================================] 1 VUs  00m00.0s/10m0s  1/1 iters, 1 per VU
