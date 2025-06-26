---
layout: home
title: "Welcome"
---

<!-- Typing animation -->
<h1>
  <a href="" class="typewrite" data-period="2000" data-type='[ "Hi there 👋, I\'m Abdul Rahman", "AI Engineer", "Deep Learning", "Computer Vision", "LLMs", "Vision-Language Models" ]'>
    <span class="wrap"></span>
  </a>
</h1>

<style>
  .typewrite > .wrap {
    border-right: 0.08em solid #000;
  }
</style>

<script>
  var TxtType = function(el, toRotate, period) {
      this.toRotate = toRotate;
      this.el = el;
      this.loopNum = 0;
      this.period = parseInt(period, 10) || 2000;
      this.txt = '';
      this.tick();
      this.isDeleting = false;
  };

  TxtType.prototype.tick = function() {
      var i = this.loopNum % this.toRotate.length;
      var fullTxt = this.toRotate[i];

      this.txt = this.isDeleting
        ? fullTxt.substring(0, this.txt.length - 1)
        : fullTxt.substring(0, this.txt.length + 1);

      this.el.innerHTML = '<span class="wrap">'+this.txt+'</span>';

      const delta = this.isDeleting ? 100 : 200 - Math.random() * 100;
      const next = this.txt === fullTxt && !this.isDeleting
        ? this.period
        : this.isDeleting && this.txt === ''
        ? (this.isDeleting = false, this.loopNum++, 500)
        : delta;

      setTimeout(() => this.tick(), next);
  };

  window.onload = function() {
      document.querySelectorAll('.typewrite').forEach((el) => {
          const toRotate = el.getAttribute('data-type');
          const period = el.getAttribute('data-period');
          if (toRotate) {
              new TxtType(el, JSON.parse(toRotate), period);
          }
      });
  };
</script>

---

## 👨‍💻 About Me

I’m an AI Engineer at **Siemens Healthineers**, focused on building intelligent systems in the healthcare domain. With a strong background in **deep learning**, **vision-language models**, and **full-stack AI deployment**, I specialize in:

- Training and fine-tuning models for **medical image analysis**
- Developing **real-time computer vision applications** (YOLO, CLIP, ResNet)
- Visualizing system performance using **Power BI and Grafana**
- Creating **web-based AI tools** using Django, REST APIs, and modern front-end

---

## 🧠 Technical Skills

- **ML/DL**: PyTorch, TensorFlow, Transformers, LLMs, CNNs, RNNs
- **Computer Vision**: YOLOv3/v8, ResNet, EfficientNet, CLIP
- **Deployment**: Django, REST APIs, HTML/CSS/JS
- **Visualization**: Power BI, Tableau, Grafana
- **Languages**: Python, JavaScript, C#, Java, C++

---

## 🔬 Projects & Research

- 🧠 **Skin Cancer Detection App**  
  Built with PyTorch + ResNet50, deployed with Django + REST API for real-time prediction.

- 🔍 **Prompt Tuning of CLIP for VLMs**  
  MSc thesis focused on few-shot adaptation across 11 datasets using lightweight adapters.

- 🚗 **Real-time Object Detection with YOLO**  
  Applied for safety monitoring (smoke/fire) and vehicle tracking.

- ⚙️ **Medical Data Analytics Dashboards**  
  Built with Power BI to optimize CT machine operations and reduce energy use.

---

## 🌍 Education & Language Skills

- 🇩🇪 MSc in Machine Learning & AI – **FAU Erlangen-Nürnberg**
- 🇨🇳 Mandarin Language Studies – **Shanghai University**
- 🇵🇰 B.E. in Embedded Software – **Federal Urdu University**

🗣️ Languages: English (C1), Mandarin (C1), German (B1→B2), Urdu, Hindi

---

## 📫 Contact Me

📧 [abdulrahman.ashraf@gmail.com](mailto:abdulrahman.ashraf@gmail.com)  
💼 [LinkedIn](https://www.linkedin.com/in/YOUR-LINKEDIN-ID)  
👨‍💻 [GitHub](https://github.com/abdulrahman45284528)

---

🟢 _I'm open to collaborations in AI research, startup innovation, and applied machine learning systems._

