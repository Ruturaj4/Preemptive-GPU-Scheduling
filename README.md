<!DOCTYPE html>
<html>
  <head>
    <h1>Preemptive GPU Scheduling - patched source code 💯</h1>
    <p>This is re-implementation of an original paper - <b> A GPU Kernel Transactionization Scheme
    for Preemptive Priority Scheduling<a href = "https://github.com/Hyunsu-Lee/psched_gpu">[1]</a></b></p>
    <p>Project Team members (University of Kansas🔶🔷)-<br><b><a href = "https://github.com/Ruturaj4">Ruturaj Vaidya</a> and <a href = "https://github.com/DhwaniPandya">Dhwani Pandya</a></b>.</p>
  </head>

  <body>
    <h2>Why GPU?</h2>
    <p>Our interest and curiosity in GPU management motivated and inspired us to work on GPU management. In todays digital
world role of GPU is crucial and the graphical data which is processed by GPU cannot be handled by CPU. Hence, GPU
aide helps in performance improvement and better resource utilization. We believe that introduction of GPU in processing
environment is triumph in itself, and this is the reason that stimulated us to pick this paper.</p>
    <h2>Project Description</h2>
    <p>Mission-critical systems simultaneously run multiple tasks with different criticality and timeliness requirements, and are becoming    heavily dependent on graphics processing unit (GPU) computing<a href = "https://github.com/Hyunsu-Lee/psched_gpu">[1]</a>. Consequently, many research efforts have been made to support the preemptive priority scheduling of GPU kernels. We re-implemented the paper, ’A GPU Kernel Transactionization Scheme for Preemptive Priority Scheduling’, which presents an approach to transactionize GPU kernels at the operating system (OS) level. By transactionizing GPU kernels, it is possible to forcibly evict low-priority kernels and immediately schedule high-priority kernels<a href = "https://github.com/Hyunsu-Lee/psched_gpu">[1]</a>.</p>
    <p>We used Odroid XU4 board for the implementation, although authors implemented on odroid XU3. We followed instructions given by authors <a href = "https://github.com/Hyunsu-Lee/psched_gpu">here</a>. However, the kernel build was unsucessful. Thus, we fixed the patch and re-built the kernel sucessfully. Thanks to our team work (and hard work indeed 😁)!</p>
    <h2>Usage (Reference: <a href = "https://github.com/Hyunsu-Lee/psched_gpu">Authors Github page</a>)</h2>
    <ul>
    <li>Download Kernel version 3.10.y from the hardkernel page</li>
    <code>git clone https://github.com/hardkernel/linux.git -b odroidxu3-3.10.y</code><br><br>
    <li>Hard reset to version 3.10.54 (As authors suggested)</li>
    <code>git reset --hard 8df9b10b63</code><br><br>
    <li>Copy the patched files to appropriate locations.</li><br>
    <li>Follow the odroid Kernel Build instructions <a href = "https://github.com/umiddelb/armhf/wiki/How-To-compile-a-custom-Linux-kernel-for-your-ARM-device">here</a>.</li>
    </ul>
    <h2>References</h2>
    <h4><a href = "https://github.com/Hyunsu-Lee/psched_gpu">[1]</a> Authors of the original paper - Hyeonsu Lee, Jaehun Roh, Euiseong Seo</h4>
    <p>School of Software, Sungkyunkwan University
    Seobu 2066, Suwon-si, Gyeonggi-do 23185, Rep. of Korea
    Email: hyeonsu.lee@csl.skku.edu, jaehun@csl.skku.edu, euiseong@skku.edu</p>
    <p> <b>Check Hyunsu-Lee's Github repository for full code</b> - https://github.com/Hyunsu-Lee/psched_gpu </p>
  </body>
</html>
