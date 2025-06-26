---
layout: home
title: "Welcome"
---

<!-- Animated intro (optional, can be removed) -->
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

      if (this.isDeleting) {
          this.txt = fullTxt.substring(0, this.txt.length - 1);
      } else {
          this.txt = fullTxt.substring(0, this.txt.length + 1);
      }

      this.el.innerHTML = '<span class="wrap">'+this.txt+'</span>';

      var that = this;
      var delta = 200 - Math.random() * 100;
      if (this.isDeleting) { delta /= 2; }

      if (!this.isDeleting && this.txt === fullTxt) {
          delta = this.period;
          this.isDeleting = true;
      } else if (this.isDeleting && this.txt === '') {
          this.isDeleting = false;
          this.loopNum++;
          delta = 500;
      }

      setTimeout(function() { that.tick(); }, delta);
  };

  window.onload = function() {
      var elements = document.getElementsByClassName('typewrite');
      for (var i=0; i<elements.length; i++) {
          var toRotate = elements[i].getAttribute('data-type');
          var period = elements[i].getAttribute('data-period');
          if (toRotate) {
              new TxtType(elements[i], JSON.parse(toRotate), period);
          }
      }
  };
</script>

---

## 👨‍💻 About Me

AI Engineer at **Siemens Healthineers**, building real-time deep learning solutions for healthcare and diagnostics. I work on model optimization, data-driven dashboards, and vision-language research.

---

## 🔧 Skills at a Glance

- **AI & Deep Learning**: GPT, BERT, CLIP, YOLO, CNNs  
- **Tech Stack**: Python, PyTorch, TensorFlow, Django, REST APIs  
- **Visualization**: Power BI, Grafana, Tableau  
- **Deployment**: Full-stack AI apps for real-world use

---

## 🧪 Key Projects

- **Skin Cancer Detector** – ResNet50 + EfficientNet with Django API  
- **CLIP Prompt Tuning** – Thesis on domain adaptation across 11 datasets  
- **YOLO Detection** – Real-time systems for safety and traffic tracking  
- **Medical Dashboards** – CT log analytics with Power BI

---

## 🌍 Background

🇩🇪 MSc in AI – FAU Erlangen-Nürnberg  
🇨🇳 Mandarin Studies – Shanghai University  
🇵🇰 B.E. in Embedded Systems – Federal Urdu University

---

## 📬 Contact

📧 [abdulrahman.ashraf@gmail.com](mailto:abdulrahman.ashraf@gmail.com)  
💼 [LinkedIn](https://www.linkedin.com/in/YOUR-LINKEDIN-ID)  
👨‍💻 [GitHub](https://github.com/abdulrahman45284528)

---

Explore the [About Page](/about/) or scroll down for featured posts and experiments.
