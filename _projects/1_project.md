---
layout: page
title: eBPF Sandbox
description: process isolation using kernel function
img: assets/img/ebpf.png
importance: 1
category: work
related_publications: true
---

Sandboxing is a process isolation technique that employs containers as streamlined, segregated environments. These containers encapsulate a program's execution along with only the essential resources required, ensuring complete compartmentalization. This setup allows each container to function independently, separate from both the host system and other containers. Essentially, sandboxing can be viewed as a form of virtualization, albeit without the need for specialized hardware or a hypervisor.

    ---
    layout: page
    title: project
    description: a project with a background image
    img: /assets/img/12.jpg
    ---

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/1.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/3.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/5.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
To understand eBPF it is important to see why it was invented. Linux began integrating advanced security and resource management features in kernel 2.x, including namespaces, root capabilities, control groups (cgroups), pivot root, and mandatory access control (MAC). These features enhanced process isolation, resource management, and system security, laying the foundation for modern containerization and virtualization technologies.

Kernel namespaces, introduced around kernel 2.6.19, abstract system-wide resources into isolated layers. Processes within a namespace perceive unique versions of resources like the processor, while changes remain hidden from others outside. This is widely used in containers and virtualization to ensure separation and compartmentalization.

Root capabilities evolved from traditional Unix privilege models, where root (UID 0) had unrestricted access. Starting with kernel 2.2, root privileges were refined into capabilities, breaking them into granular levels. This allowed specific permissions to be assigned to processes, enhancing security by limiting excessive access.

Control groups (cgroups), developed by Google engineers, organize processes hierarchically. They enable resource restrictions and monitoring, such as CPU, memory, disk, and I/O limits, without the application’s awareness. This ensures efficient resource allocation and prevents processes from overusing system resources.

Pivot root allows users with specific capabilities to change the root mount point in a containerized environment. MAC enforces stricter access rules than DAC, granting resources only with explicit authorization. For example, a webserver might access only port 80 and specific folders, enhancing system security and resource control.
</div>
<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/5.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    This image can also have a caption. It's like magic.
</div>

You can also put regular text between your rows of images, even citations {% cite einstein1950meaning %}.
Say you wanted to write a bit about your project before you posted the rest of the images.
You describe how you toiled, sweated, _bled_ for your project, and then... you reveal its glory in the next row of images.

<div class="row justify-content-sm-center">
    <div class="col-sm-8 mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/6.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm-4 mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/11.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    You can also have artistically styled 2/3 + 1/3 images, like these.
</div>

The code is simple.
Just wrap your images with `<div class="col-sm">` and place them inside `<div class="row">` (read more about the <a href="https://getbootstrap.com/docs/4.4/layout/grid/">Bootstrap Grid</a> system).
To make images responsive, add `img-fluid` class to each; for rounded corners and shadows use `rounded` and `z-depth-1` classes.
Here's the code for the last row of images above:

{% raw %}

```html
<div class="row justify-content-sm-center">
  <div class="col-sm-8 mt-3 mt-md-0">
    {% include figure.liquid path="assets/img/6.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
  </div>
  <div class="col-sm-4 mt-3 mt-md-0">
    {% include figure.liquid path="assets/img/11.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
  </div>
</div>
```

{% endraw %}
