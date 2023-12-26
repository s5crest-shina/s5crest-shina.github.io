---
title: 'ORC: Increasing Cloud Memory Density via Object Reuse with Capabilities'
authors:
  - Vasily A. Sartakov
  - Lluís Vilanova
  - Munir Geden
  - David Eyers
  - Takahiro Shinagawa
  - Peter Pietzuch
date: '2023-07-11T00:00:00Z'
publication_types: ['conference']
publication: In Proceedings of the 17th USENIX Symposium on Operating Systems Design and Implementation
doi: ''

abstract: 'Cloud environments host many tenants, and typically there is substantial overlap between the application binaries and libraries executed by tenants. Thus, memory de-duplication can increase memory density by allocating memory for shared binaries only once. Existing de-duplication approaches, however, either rely on a shared OS to de-deduplicate binary objects, which provides unacceptably weak isolation; or exploit hypervisor-based de-duplication at the level of memory pages, which is blind to the semantics of the objects to be shared.<br>
<br>
We describe Object Reuse with Capabilities (ORC), which supports the fine-grained sharing of binary objects between tenants, while isolating tenants strongly through a small trusted computing base (TCB). ORC uses hardware support for memory capabilities to isolate tenants, which permits shared objects to be accessible to multiple tenants safely. Since ORC shares binary objects within a single address space through capabilities, it uses a new relocation type to create per-tenant state when loading shared objects. ORC supports the loading of objects by an untrusted guest, outside of its TCB, only verifying the safety of the loaded data. Our experiments show that ORC achieves a higher memory density with a lower overhead than hypervisor-based de-deduplication.'

# Summary. An optional shortened abstract.
summary: ''

tags: []

# Display this page in the Featured widget?
featured: false

# Custom links (uncomment lines below)
# links:
# - name: Custom Link
#   url: http://example.org

url_pdf: 'https://www.usenix.org/system/files/osdi23-sartakov.pdf'
url_code: ''
url_dataset: ''
url_poster: ''
url_project: ''
url_slides: 'https://www.usenix.org/system/files/osdi23_slides_sartakov.pdf'
url_source: ''
url_video: 'https://youtu.be/vJDFODprL9E'

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
