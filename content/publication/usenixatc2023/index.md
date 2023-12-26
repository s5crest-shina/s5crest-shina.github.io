---
title: 'Translation Pass-Through for Near-Native Paging Performance in VMs'
authors:
  - Shai Bergman
  - Mark Silberstein
  - Takahiro Shinagawa
  - Peter Pietzuch
  - Lluís Vilanova
date: '2023-07-12T00:00:00Z'
publication_types: ['conference']
publication: In Proceedings of the 2023 USENIX Annual Technical Conference (USENIX ATC 2023)
doi: ''

abstract: 'Virtual machines~(VMs) are used for consolidation, isolation, and provisioning in the cloud, but applications with large working sets are impacted by the overheads of memory address translation in VMs. Existing translation approaches incur non-trivial overheads: (i)~nested paging has a worst-case latency that increases with page table depth; and (ii)~paravirtualized and shadow paging suffer from high hypervisor intervention costs when updating guest page tables.<br>
<br>
We describe Translation Pass-Through (TPT), a new memory virtualization mechanism that achieves near-native performance. TPT enables VMs to control virtual memory translation from guest-virtual to host-physical addresses using one-dimensional page tables. At the same time, inter-VM isolation is enforced by the host by exploiting new hardware support for physical memory tagging in commodity CPUs.<br>
<br>
We prototype TPT by modifying the KVM/QEMU hypervisor and enlightening the Linux guest. We evaluate it by emulating the memory tagging mechanism of AMD CPUs. Our conservative performance estimates show that TPT achieves native performance for real-world data center applications, with speedups of up to 2.4× and 1.4× over nested and shadow paging, respectively.'

# Summary. An optional shortened abstract.
summary: ''

tags: []

# Display this page in the Featured widget?
featured: false

# Custom links (uncomment lines below)
# links:
# - name: Custom Link
#   url: http://example.org

url_pdf: 'https://www.usenix.org/system/files/atc23-bergman.pdf'
url_code: ''
url_dataset: ''
url_poster: ''
url_project: ''
url_slides: 'https://www.usenix.org/system/files/atc23_slides_bergman.pdf'
url_source: ''
url_video: 'https://youtu.be/e1DrrIKU0Ko'

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder.
#image:
#  caption: ''
#  focal_point: ''
#  preview_only: false

# Associated Projects (optional).
#   Associate this publication with one or more of your projects.
#   Simply enter your project's folder or file name without extension.
#   E.g. `internal-project` references `content/project/internal-project/index.md`.
#   Otherwise, set `projects: []`.
projects:
  - FrieOS

# Slides (optional).
#   Associate this publication with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides: "example"` references `content/slides/example/index.md`.
#   Otherwise, set `slides: ""`.
slides: ""
---
