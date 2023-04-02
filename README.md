# Certified-Kubernetes-Security-Specialist
<p align="center">
    <img width="200" src="https://user-images.githubusercontent.com/46586312/228611431-70b2a3ad-5e7c-4bec-9a55-3890db4ac67b.png" alt="Material Bread logo">
</p>



The CKS certification is designed to validate an individual's understanding of Kubernetes security principles and best practices, as well as the ability to secure Kubernetes clusters and workloads. CKS certified professionals are expected to have a deep understanding of Kubernetes security concepts, network security, access management, and secure container image management.

Having a CKS certification can help individuals stand out in the job market and demonstrate their expertise to potential employers. It can also give them the confidence and credibility to perform Kubernetes security assessments and audits for organizations. Additionally, organizations may choose to hire CKS certified professionals to ensure that their Kubernetes environments are secure and compliant with industry standards.

As someone who has taken the CKS exam, I recommend reviewing the exam blueprint thoroughly and understanding the concepts behind each objective. It's also important to read the questions carefully and pay attention to any specific details or requirements mentioned.

Lastly, time management is key during the exam. Make sure to allocate enough time for each question and don't spend too much time on any one question. If you're unsure about a question, flag it and come back to it later.

Overall, with the right resources and preparation, the CKS exam can be successfully passed. 

I will share some tips that may help prepare for your CKS exam.

## Contents
1. [What I used to review](#whatiused)
2. [Helpful Resources](#helpfulresources)
3. [Topics](#topics)
4. [Exam Environment](#examenvironment)
5. [Allowed documentations during the exam](#alloweddocs) 
6. [My Study Guide](#mystudyguide)

# What I used to review <a name="whatiused"></a>
 1. [Kodekloud's CKS Course](https://kodekloud.com/courses/certified-kubernetes-security-specialist-cks/)
  
    Kodekloud's Certified Kubernetes Security Specialist (CKS) course is a comprehensive learning resource for individuals who want to prepare for the CKS certification exam. The course covers a wide range of topics related to Kubernetes security, including cluster hardening, access management, network security, and secure container image management.

    The Kodekloud CKS course is helpful because it provides a structured learning path and hands-on exercises that enable learners to gain a practical understanding of Kubernetes security concepts. The course includes video lectures, quizzes, and practical exercises that simulate real-world scenarios, which can help learners develop the skills needed to secure Kubernetes environments.

    ### Here are some improved strategies I followed to effectively learn the course:

    **Create a study schedule:** I created a detailed study schedule that spanned 1.5 months, dedicating an average of 2 hours per day to study. I made sure to stick to the schedule as closely as possible to ensure that I covered all the material in a timely and efficient manner.

    **Take detailed notes:** While watching the video lectures, I took detailed notes to help me retain information and better understand the concepts. I made sure to include examples and explanations to ensure that I fully understood the material.

    **Practice lab exercises and mock exams:** To reinforce my learning, I practiced the lab exercises multiple times and took the mock exams 3-4 times until I felt confident with the material. If I couldn't answer certain questions, I went back to the topic or did further research to better understand it. Additionally, I found a [Github link](https://github.com/kodekloudhub/certified-kubernetes-security-specialist-cks-course/tree/main/docs/08-Mock-Exams) that shared how the questions could be answered, which helped me gain a better understanding of how to solve the questions.

    **Engage in the Kodekloud slack community:** I joined [Kodekloud's slack community](https://join.slack.com/t/kodekloud/shared_invite/zt-wm5xso39-L1xVR2yWdy9uPg_jk4wRwA) , where I could ask questions, share my knowledge, and discuss concepts with other learners. The community was a great resource for me, as I was able to receive feedback from other learners and learn from their experiences as well.

    By following these strategies, I was able to effectively learn the course material and gain a solid understanding of the concepts.


2. [Killercoda's Interactive Test Simulators](https://killercoda.com/killer-shell-cks)

    One helpful resource I used to prepare for the CKS exam was the test scenarios provided by Killercoda. With over 50 scenarios available, practicing them provided me with a new set of questions that weren't available in Kodekloud's resources. I practiced all the scenarios 2-3 times to reinforce my understanding of the material and ensure I was fully prepared for the exam. The scenarios were especially helpful as they provided me with real-world examples and challenges that helped me develop my problem-solving skills and better understand the practical applications of the concepts I had learned. Overall, I found Killercoda's test scenarios to be an invaluable resource for CKS exam preparation.

3. [Killer.sh](https://killer.sh/cks)

    When you purchase a voucher for the CKS exam, it comes with 2 killer.sh sessions. These sessions provide an exam simulator that closely mirrors the actual exam environment. This tool is incredibly useful for familiarizing yourself with the exam format and ensuring you are comfortable with the tools and settings, such as setting up your terminal window and browser.

    I found that the questions on killer.sh were slightly more challenging than those on the actual exam, making it a great tool to gauge your readiness for the exam. With unlimited resets and a 36-hour access window, I practiced all the questions 2-3 times until I achieved a "fair" result. Additionally, the tool provides solutions to the questions, which gave me a better understanding of how to approach and solve similar problems.

    Overall, killer.sh is a valuable resource for anyone preparing for the CKS exam, providing a realistic simulation of the exam environment and challenging questions to help you prepare for success on exam day.

# Helpful Resources <a name="helpfulresources"></a>

1. https://kubernetes.io/docs - 
2. https://orca.tufin.io/netpol/ - You can get your network policies explained by pasting it into this tool.
3. https://vim.rtorr.com/ - Getting yourself familiarized with the vi shortcuts would help you make change the configurations faster.

# Topics <a name="topics"></a>
### Cluster Setup 10%
> - Use Network security policies to restrict cluster level access
> - Use CIS benchmark to review the security configuration of Kubernetes components (etcd, kubelet, kubedns, kubeapi)
> - Properly set up Ingress objects with security control
> - Protect node metadata and endpoints
> - Minimize use of, and access to, GUI elements
> - Verify platform binaries before deploying

### Cluster Hardening 15%
> - Restrict access to Kubernetes API
> - Use Role Based Access Controls to minimize exposure
> - Exercise caution in using service accounts e.g. disable defaults, minimize permissions on newly created ones
> - Update Kubernetes frequently

### System Hardening 15%
> - Minimize host OS footprint (reduce attack surface)
> - Minimize IAM roles
> - Minimize external access to the network
> - Appropriately use kernel hardening tools such as AppArmor, seccomp

### Minimize Microservice Vulnerabilities 20%
> - Setup appropriate OS level security domains
> - Manage Kubernetes secrets
> - Use container runtime sandboxes in multi-tenant environments (e.g. gvisor, kata containers)
> - Implement pod to pod encryption by use of mTLS

### Supply Chain Security 20% 
> - Minimize base image footprint
> - Secure your supply chain: whitelist allowed registries, sign and validate images
> - Use static analysis of user workloads (e.g.Kubernetes resources, Docker files)
> - Scan images for known vulnerabilities

### Monitoring, Logging and Runtime Security 20%
> - Perform behavioral analytics of syscall process and file activities at the host and container level to detect malicious activities
> - Detect threats within physical infrastructure, apps, networks, data, users and workloads
> - Detect all phases of attack regardless where it occurs and how it spreads
> - Perform deep analytical investigation and identification of bad actors within environment
> - Ensure immutability of containers at runtime
> - Use Audit Logs to monitor access

# Exam Environment <a name="examenvironment"></a>

### Practice the exam environment: 
If you have access to killer.sh exam simulator, take some time to familiarize yourself with it. This can help you feel more comfortable and confident during the actual exam.

Linux Foundation prepared some sample UI of the exam environment and given some tips on this link: 
https://docs.linuxfoundation.org/tc-docs/certification/lf-handbook2/exam-user-interface/examui-performance-based-exams

### Quick glance on it looks like: 
![Alt text](LF%20Remote%20Desktop%20070722d.png)
*(image from Linux Foundation)*

# Allowed documentations during the exam <a name="alloweddocs"></a>
**Kubernetes Documentation:**
https://kubernetes.io/docs/ and their subdomains
https://kubernetes.io/blog/ and their subdomains
This includes all available language translations of these pages (e.g. https://kubernetes.io/zh/docs/)

**Trivy documentation** https://aquasecurity.github.io/trivy/

**Falco documentation** https://falco.org/docs/
This includes all available language translations of these pages (e.g. https://falco.org/zh/docs/)

**App Armor:**
Documentation https://gitlab.com/apparmor/apparmor/-/wikis/Documentation

# My Study Guide <a name="mystudyguide"></a>

*updating the blog in progress*