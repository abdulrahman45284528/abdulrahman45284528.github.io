---
layout: home
title: "Welcome"
---

# 👋 Hello, I'm Abdul Rahman

<!-- Typing animation section -->
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

      setTimeout(function() {
          that.tick();
      }, delta);
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


Currently working at **Siemens Healthineers** in Germany, I specialize in:
- Designing and optimizing **deep learning pipelines** for medical imaging
- Building **interactive analytics dashboards** from CT scanner telemetry
- Deploying robust **AI applications** using PyTorch, TensorFlow, and Django

---

## 🔬 My Technical Focus

- **Deep Learning & Transformers**: GPT, BERT, CLIP, CNNs, RNNs
- **Computer Vision**: Object detection with YOLO, image classification with ResNet, segmentation with EfficientNet
- **Vision–Language Models (VLMs)**: Prompt tuning, domain adaptation, and few-shot learning
- **Full-Stack AI Deployment**: Python | REST API | Django | Frontend (HTML/CSS/JS)
- **Visualization & Monitoring**: Power BI | Grafana | Tableau | Azure Databricks

---

## 📈 Featured Projects

- 🧠 **Skin Cancer Detection App**  
  Web-based real-time lesion classification using PyTorch, ResNet50, and EfficientNet  
  → Full-stack deployed with Django and REST API

- 🔍 **Prompt Tuning for Vision–Language Models**  
  Master’s thesis on adapting CLIP across 11 datasets under few-shot conditions  
  → Improved generalization with lightweight adapters and gradient regularization

- 🚗 **YOLO Object Detection Systems**  
  Real-time detection for smoke, fire hazards, and license plates  
  → Boosting safety and traffic analytics in live environments

- ⚙️ **Medical Data Visualization**  
  Created dashboards using Power BI for CT scanner operations  
  → Identified gaps, optimized energy use, and improved reliability

---

## 🌍 Global Experience & Education

- 🇩🇪 **Germany**: MSc in AI/ML – FAU Erlangen-Nürnberg  
- 🇨🇳 **China**: Mandarin language and culture studies – Shanghai University  
- 🇵🇰 **Pakistan**: Bachelor's in Embedded Software Design

---

## 📫 Let's Connect

- 📧 [abdulrahman.ashraf@gmail.com](mailto:abdulrahman.ashraf@gmail.com)  
- 💼 [LinkedIn](https://www.linkedin.com/in/YOUR-LINKEDIN-ID)  
- 👨‍💻 [GitHub](https://github.com/abdulrahman45284528)

---

🟢 _I’m always excited to collaborate on innovative AI projects, research applications, or intelligent products that make an impact._  
Explore my [About Page](/about/) or scroll below for blog posts and experiments.
