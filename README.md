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

# What I used to review
1. [Kodekloud's CKS Course](https://kodekloud.com/courses/certified-kubernetes-security-specialist-cks/)
  
Kodekloud's Certified Kubernetes Security Specialist (CKS) course is a comprehensive learning resource for individuals who want to prepare for the CKS certification exam. The course covers a wide range of topics related to Kubernetes security, including cluster hardening, access management, network security, and secure container image management.

The Kodekloud CKS course is helpful because it provides a structured learning path and hands-on exercises that enable learners to gain a practical understanding of Kubernetes security concepts. The course includes video lectures, quizzes, and practical exercises that simulate real-world scenarios, which can help learners develop the skills needed to secure Kubernetes environments.

Here are some strategies I followed to effectively learn the course:

- **Plan a study schedule:** I have prepared for 1.5 months and have spent 2 hours daily _(on an average)_ to study. 

- **Take notes:** I find taking notes helpful while watching the video lectures. It helped me retain information and better understand the concepts.

- **Practice the lab exercises and mock exams:**  I practiced the lab exercises twice and took the mock exams 3-4 times until I felt confident about the topic. If I couldn't answer certain questions, I would go back to the topic or do further research to better understand it. The mock exams don't come with answers that you can reference with, but I found this [Github link](https://github.com/kodekloudhub/certified-kubernetes-security-specialist-cks-course/tree/main/docs/08-Mock-Exams) that shares how the questions can be answered. It will help give you an idea on how to solve the questions.

- **Ask questions in Kodekloud's slack community:** Kodekloud has a great [slack community](https://join.slack.com/t/kodekloud/shared_invite/zt-wm5xso39-L1xVR2yWdy9uPg_jk4wRwA) where you can ask questions, share your knowledge, and discuss concepts with other learners. 

2. [Killercoda's Interactive Test Simulators](https://killercoda.com/killer-shell-cks)

Killercoda really have helpful test scenarios that can be used as well for the CKS preparation. They have around 50+ scenarios available that you may use to practice and would give you new set of questions that won't be available in Kodekloud's. I've practiced all the scenarios 2-3 times.

3. [Killer.sh](https://killer.sh/cks)

When you buy a voucher for the CKS exam, it comes with 2 killer.sh sessions. killer.sh will give an exam simulator that is similar to what you will be having on the actual exam. It is very useful to help familiarize yourself on the exam environment, like to setup your terminal window, browser, etc..

I would say killer.sh has tougher questions than the actual exam. This is a best practice to know if you are ready to take the exam or not. You may use it for 36 hours with unlimited resets. I've practiced all the questions 2-3 times until I got a "fair" result. You will have an option to see the solutions as well, to give you an idea how the questions are answered.

# Helpful Resources

1. https://orca.tufin.io/netpol/ - You can get your network policies explained by pasting it into this tool.

# Topics
## Cluster Setup 10%
> - Use Network security policies to restrict cluster level access
> - Use CIS benchmark to review the security configuration of Kubernetes components (etcd, kubelet, kubedns, kubeapi)
> - Properly set up Ingress objects with security control
> - Protect node metadata and endpoints
> - Minimize use of, and access to, GUI elements
> - Verify platform binaries before deploying

## Cluster Hardening 15%
> - Restrict access to Kubernetes API
> - Use Role Based Access Controls to minimize exposure
> - Exercise caution in using service accounts e.g. disable defaults, minimize permissions on newly created ones
> - Update Kubernetes frequently

## System Hardening 15%
> - Minimize host OS footprint (reduce attack surface)
> - Minimize IAM roles
> - Minimize external access to the network
> - Appropriately use kernel hardening tools such as AppArmor, seccomp

## Minimize Microservice Vulnerabilities 20%
> - Setup appropriate OS level security domains
> - Manage Kubernetes secrets
> - Use container runtime sandboxes in multi-tenant environments (e.g. gvisor, kata containers)
> - Implement pod to pod encryption by use of mTLS

## Supply Chain Security 20% 
> - Minimize base image footprint
> - Secure your supply chain: whitelist allowed registries, sign and validate images
> - Use static analysis of user workloads (e.g.Kubernetes resources, Docker files)
> - Scan images for known vulnerabilities

## Monitoring, Logging and Runtime Security 20%
> - Perform behavioral analytics of syscall process and file activities at the host and container level to detect malicious activities
> - Detect threats within physical infrastructure, apps, networks, data, users and workloads
> - Detect all phases of attack regardless where it occurs and how it spreads
> - Perform deep analytical investigation and identification of bad actors within environment
> - Ensure immutability of containers at runtime
> - Use Audit Logs to monitor access
