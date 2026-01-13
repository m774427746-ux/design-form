[index (3).html](https://github.com/user-attachments/files/24580238/index.3.html)
<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
<meta charset="UTF-8">
<title>نموذج طلب مشروع تصميم - احترافي</title>
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<!-- Cairo Font - Premium Arabic -->
<link href="https://fonts.googleapis.com/css2?family=Cairo:wght@300;400;600;700;900&display=swap" rel="stylesheet">

<!-- Feather Icons -->
<script src="https://unpkg.com/feather-icons"></script>

<style>
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

:root {
  --primary: #6366f1;
  --primary-dark: #4f46e5;
  --primary-light: #818cf8;
  --secondary: #06b6d4;
  --accent: #f59e0b;
  --success: #10b981;
  --danger: #ef4444;
  --dark: #1e293b;
  --text: #334155;
  --text-light: #64748b;
  --bg: #ffffff;
  --bg-light: #f8fafc;
  --border: #e2e8f0;
  --shadow: rgba(0, 0, 0, 0.1);
}

body {
  font-family: 'Cairo', sans-serif;
  background: linear-gradient(135deg, #f8fafc 0%, #e0e7ff 100%);
  color: var(--text);
  min-height: 100vh;
  padding: 40px 20px;
  position: relative;
  overflow-x: hidden;
}

/* Animated Background Shapes */
.bg-shapes {
  position: fixed;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  z-index: 0;
  overflow: hidden;
  pointer-events: none;
}

.shape {
  position: absolute;
  border-radius: 50%;
  filter: blur(80px);
  opacity: 0.3;
  animation: float 20s ease-in-out infinite;
}

.shape-1 {
  width: 500px;
  height: 500px;
  background: linear-gradient(135deg, #6366f1, #818cf8);
  top: -150px;
  left: -150px;
  animation-delay: 0s;
}

.shape-2 {
  width: 400px;
  height: 400px;
  background: linear-gradient(135deg, #06b6d4, #0891b2);
  bottom: -100px;
  right: -100px;
  animation-delay: 7s;
}

.shape-3 {
  width: 300px;
  height: 300px;
  background: linear-gradient(135deg, #f59e0b, #fbbf24);
  top: 40%;
  right: 10%;
  animation-delay: 14s;
}

@keyframes float {
  0%, 100% {
    transform: translate(0, 0) rotate(0deg);
  }
  33% {
    transform: translate(50px, -80px) rotate(120deg);
  }
  66% {
    transform: translate(-40px, 60px) rotate(240deg);
  }
}

/* Container */
.container {
  max-width: 900px;
  margin: 0 auto;
  position: relative;
  z-index: 1;
}

/* Header */
.header {
  text-align: center;
  margin-bottom: 60px;
  animation: fadeInDown 0.8s cubic-bezier(0.34, 1.56, 0.64, 1);
}

.logo {
  width: 80px;
  height: 80px;
  margin: 0 auto 30px;
  background: linear-gradient(135deg, var(--primary), var(--secondary));
  border-radius: 20px;
  display: flex;
  align-items: center;
  justify-content: center;
  box-shadow: 0 20px 60px rgba(99, 102, 241, 0.4);
  animation: logoFloat 3s ease-in-out infinite;
  position: relative;
}

.logo::before {
  content: '';
  position: absolute;
  width: 100%;
  height: 100%;
  border-radius: 20px;
  background: linear-gradient(135deg, var(--primary), var(--secondary));
  animation: pulse 2s ease-in-out infinite;
  z-index: -1;
}

@keyframes logoFloat {
  0%, 100% { transform: translateY(0px); }
  50% { transform: translateY(-10px); }
}

@keyframes pulse {
  0%, 100% { transform: scale(1); opacity: 0.8; }
  50% { transform: scale(1.1); opacity: 0.5; }
}

.logo svg {
  width: 40px;
  height: 40px;
  stroke: white;
  stroke-width: 2;
}

h1 {
  font-size: 42px;
  font-weight: 900;
  color: var(--dark);
  margin-bottom: 15px;
  letter-spacing: -1px;
}

.subtitle {
  font-size: 18px;
  color: var(--text-light);
  max-width: 600px;
  margin: 0 auto;
  line-height: 1.7;
}

@keyframes fadeInDown {
  from {
    opacity: 0;
    transform: translateY(-50px);
  }
  to {
    opacity: 1;
    transform: translateY(0);
  }
}

/* Form Card */
.form-card {
  background: rgba(255, 255, 255, 0.95);
  backdrop-filter: blur(20px);
  border-radius: 30px;
  padding: 50px;
  box-shadow: 
    0 20px 60px rgba(0, 0, 0, 0.08),
    0 0 0 1px rgba(0, 0, 0, 0.05);
  animation: fadeInUp 0.8s cubic-bezier(0.34, 1.56, 0.64, 1) 0.2s both;
  transition: transform 0.3s ease;
}

@keyframes fadeInUp {
  from {
    opacity: 0;
    transform: translateY(50px);
  }
  to {
    opacity: 1;
    transform: translateY(0);
  }
}

/* Section */
.section {
  margin-bottom: 45px;
  animation: slideIn 0.6s ease-out both;
  animation-delay: calc(var(--section-index) * 0.1s);
}

@keyframes slideIn {
  from {
    opacity: 0;
    transform: translateX(-30px);
  }
  to {
    opacity: 1;
    transform: translateX(0);
  }
}

.section-header {
  display: flex;
  align-items: center;
  gap: 15px;
  margin-bottom: 30px;
  padding-bottom: 20px;
  border-bottom: 2px solid var(--border);
  position: relative;
}

.section-header::after {
  content: '';
  position: absolute;
  bottom: -2px;
  left: 0;
  width: 0;
  height: 2px;
  background: linear-gradient(90deg, var(--primary), var(--secondary));
  transition: width 0.6s cubic-bezier(0.34, 1.56, 0.64, 1);
}

.section:hover .section-header::after {
  width: 120px;
}

.section-icon {
  width: 50px;
  height: 50px;
  border-radius: 15px;
  display: flex;
  align-items: center;
  justify-content: center;
  transition: all 0.4s cubic-bezier(0.34, 1.56, 0.64, 1);
  position: relative;
}

.section-icon::before {
  content: '';
  position: absolute;
  width: 100%;
  height: 100%;
  border-radius: 15px;
  background: inherit;
  opacity: 0.3;
  transform: scale(0);
  transition: transform 0.4s cubic-bezier(0.34, 1.56, 0.64, 1);
}

.section:hover .section-icon::before {
  transform: scale(1.5);
}

.section:hover .section-icon {
  transform: rotate(10deg) scale(1.1);
}

.section-icon svg {
  width: 26px;
  height: 26px;
  stroke-width: 2.5;
  color: white;
  position: relative;
  z-index: 1;
}

.section:nth-child(1) .section-icon { background: linear-gradient(135deg, #6366f1, #818cf8); }
.section:nth-child(2) .section-icon { background: linear-gradient(135deg, #06b6d4, #0891b2); }
.section:nth-child(3) .section-icon { background: linear-gradient(135deg, #f59e0b, #fbbf24); }
.section:nth-child(4) .section-icon { background: linear-gradient(135deg, #10b981, #34d399); }
.section:nth-child(5) .section-icon { background: linear-gradient(135deg, #8b5cf6, #a78bfa); }
.section:nth-child(6) .section-icon { background: linear-gradient(135deg, #ef4444, #f87171); }
.section:nth-child(7) .section-icon { background: linear-gradient(135deg, #ec4899, #f472b6); }

.section-title {
  font-size: 22px;
  font-weight: 700;
  color: var(--dark);
}

/* Form Elements */
label {
  display: flex;
  align-items: center;
  gap: 8px;
  color: var(--dark);
  font-weight: 600;
  margin-bottom: 12px;
  font-size: 15px;
  transition: color 0.3s ease;
}

label svg {
  width: 18px;
  height: 18px;
  stroke-width: 2.5;
}

label.required::after {
  content: "*";
  color: var(--danger);
  margin-right: 4px;
  font-size: 18px;
}

input, textarea, select {
  width: 100%;
  padding: 14px 18px;
  border-radius: 12px;
  border: 2px solid var(--border);
  background: var(--bg);
  color: var(--dark);
  font-size: 15px;
  font-family: 'Cairo', sans-serif;
  margin-bottom: 20px;
  transition: all 0.3s cubic-bezier(0.34, 1.56, 0.64, 1);
  font-weight: 500;
}

input::placeholder, textarea::placeholder {
  color: var(--text-light);
  font-weight: 400;
}

input:focus, textarea:focus, select:focus {
  outline: none;
  border-color: var(--primary);
  background: #fafbff;
  transform: translateY(-2px);
  box-shadow: 0 8px 20px rgba(99, 102, 241, 0.15);
}

textarea {
  min-height: 120px;
  resize: vertical;
}

select {
  cursor: pointer;
  appearance: none;
  background-image: url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' width='24' height='24' viewBox='0 0 24 24' fill='none' stroke='%236366f1' stroke-width='2' stroke-linecap='round' stroke-linejoin='round'%3E%3Cpolyline points='6 9 12 15 18 9'%3E%3C/polyline%3E%3C/svg%3E");
  background-repeat: no-repeat;
  background-position: left 15px center;
  background-size: 18px;
  padding-left: 45px;
}

select option {
  background: white;
  color: var(--dark);
  padding: 12px;
}

/* Checkbox Group */
.checkbox-group {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
  gap: 15px;
  margin-bottom: 25px;
}

.checkbox-item {
  position: relative;
}

.checkbox-item input {
  position: absolute;
  opacity: 0;
  width: 0;
  height: 0;
  margin: 0;
}

.checkbox-label {
  display: flex;
  align-items: center;
  gap: 12px;
  padding: 16px 18px;
  background: var(--bg-light);
  border: 2px solid var(--border);
  border-radius: 12px;
  cursor: pointer;
  transition: all 0.3s cubic-bezier(0.34, 1.56, 0.64, 1);
  color: var(--dark);
  font-weight: 600;
  margin: 0;
}

.checkbox-label:hover {
  background: white;
  border-color: var(--primary-light);
  transform: translateY(-4px);
  box-shadow: 0 10px 25px rgba(99, 102, 241, 0.15);
}

.checkbox-item input:checked + .checkbox-label {
  background: linear-gradient(135deg, #eef2ff, #e0e7ff);
  border-color: var(--primary);
  color: var(--primary);
  box-shadow: 0 10px 30px rgba(99, 102, 241, 0.2);
}

.checkbox-icon {
  display: flex;
  align-items: center;
  justify-content: center;
  width: 36px;
  height: 36px;
  border-radius: 10px;
  background: white;
  transition: all 0.3s cubic-bezier(0.34, 1.56, 0.64, 1);
  flex-shrink: 0;
}

.checkbox-icon svg {
  width: 20px;
  height: 20px;
  stroke-width: 2.5;
  color: var(--text-light);
  transition: all 0.3s ease;
}

.checkbox-item input:checked + .checkbox-label .checkbox-icon {
  background: linear-gradient(135deg, var(--primary), var(--primary-light));
  transform: rotate(360deg) scale(1.1);
}

.checkbox-item input:checked + .checkbox-label .checkbox-icon svg {
  color: white;
}

/* Hint */
.hint {
  display: flex;
  align-items: center;
  gap: 8px;
  color: var(--text-light);
  font-size: 13px;
  margin-top: -12px;
  margin-bottom: 20px;
  font-style: italic;
}

.hint svg {
  width: 16px;
  height: 16px;
  stroke-width: 2;
}

/* Submit Button */
.submit-wrapper {
  margin-top: 50px;
  text-align: center;
}

.submit-btn {
  position: relative;
  padding: 18px 50px;
  font-size: 18px;
  font-weight: 700;
  color: white;
  border: none;
  border-radius: 15px;
  background: linear-gradient(135deg, var(--primary), var(--secondary));
  cursor: pointer;
  overflow: hidden;
  transition: all 0.4s cubic-bezier(0.34, 1.56, 0.64, 1);
  box-shadow: 0 15px 40px rgba(99, 102, 241, 0.4);
  font-family: 'Cairo', sans-serif;
  display: inline-flex;
  align-items: center;
  justify-content: center;
  gap: 12px;
  letter-spacing: 0.5px;
}

.submit-btn::before {
  content: '';
  position: absolute;
  top: 0;
  left: -100%;
  width: 100%;
  height: 100%;
  background: linear-gradient(90deg, transparent, rgba(255, 255, 255, 0.3), transparent);
  transition: left 0.6s;
}

.submit-btn:hover::before {
  left: 100%;
}

.submit-btn:hover {
  transform: translateY(-5px);
  box-shadow: 0 25px 60px rgba(99, 102, 241, 0.5);
}

.submit-btn:active {
  transform: translateY(-2px) scale(0.98);
}

.submit-btn svg {
  width: 22px;
  height: 22px;
  stroke-width: 2.5;
}

.submit-btn.loading {
  pointer-events: none;
  opacity: 0.8;
}

.submit-btn.loading::after {
  content: '';
  position: absolute;
  width: 20px;
  height: 20px;
  border: 3px solid rgba(255, 255, 255, 0.3);
  border-top-color: white;
  border-radius: 50%;
  animation: spin 0.8s linear infinite;
}

@keyframes spin {
  to { transform: rotate(360deg); }
}

/* Success Modal */
.success-modal {
  position: fixed;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  background: rgba(0, 0, 0, 0.6);
  backdrop-filter: blur(10px);
  display: none;
  align-items: center;
  justify-content: center;
  z-index: 9999;
  animation: fadeIn 0.3s ease-out;
}

.success-modal.show {
  display: flex;
}

@keyframes fadeIn {
  from { opacity: 0; }
  to { opacity: 1; }
}

.success-content {
  background: white;
  border-radius: 25px;
  padding: 60px 50px;
  text-align: center;
  max-width: 550px;
  width: 90%;
  box-shadow: 0 30px 80px rgba(0, 0, 0, 0.2);
  animation: modalBounce 0.6s cubic-bezier(0.34, 1.56, 0.64, 1);
}

@keyframes modalBounce {
  from {
    opacity: 0;
    transform: scale(0.5) translateY(50px);
  }
  to {
    opacity: 1;
    transform: scale(1) translateY(0);
  }
}

.success-icon {
  width: 90px;
  height: 90px;
  margin: 0 auto 30px;
  background: linear-gradient(135deg, var(--success), #34d399);
  border-radius: 50%;
  display: flex;
  align-items: center;
  justify-content: center;
  box-shadow: 0 15px 40px rgba(16, 185, 129, 0.3);
  animation: checkBounce 0.8s cubic-bezier(0.34, 1.56, 0.64, 1) 0.3s both;
}

@keyframes checkBounce {
  0% { transform: scale(0); }
  50% { transform: scale(1.2); }
  100% { transform: scale(1); }
}

.success-icon svg {
  width: 50px;
  height: 50px;
  stroke-width: 3;
  color: white;
}

.success-title {
  font-size: 32px;
  font-weight: 900;
  color: var(--dark);
  margin-bottom: 15px;
}

.success-message {
  font-size: 17px;
  color: var(--text);
  margin-bottom: 35px;
  line-height: 1.7;
}

.btn-close {
  padding: 14px 40px;
  border: 2px solid var(--border);
  border-radius: 12px;
  font-size: 16px;
  font-weight: 600;
  cursor: pointer;
  transition: all 0.3s ease;
  font-family: 'Cairo', sans-serif;
  background: var(--bg-light);
  color: var(--dark);
  display: inline-flex;
  align-items: center;
  gap: 10px;
}

.btn-close svg {
  width: 20px;
  height: 20px;
  stroke-width: 2.5;
}

.btn-close:hover {
  background: var(--dark);
  color: white;
  border-color: var(--dark);
  transform: translateY(-2px);
  box-shadow: 0 8px 20px rgba(0, 0, 0, 0.15);
}

/* Responsive */
@media (max-width: 768px) {
  body {
    padding: 20px 15px;
  }

  .form-card {
    padding: 35px 25px;
    border-radius: 25px;
  }

  h1 {
    font-size: 32px;
  }

  .logo {
    width: 70px;
    height: 70px;
  }

  .section {
    margin-bottom: 35px;
  }

  .section-icon {
    width: 45px;
    height: 45px;
  }

  .section-icon svg {
    width: 22px;
    height: 22px;
  }

  .section-title {
    font-size: 19px;
  }

  .checkbox-group {
    grid-template-columns: 1fr;
  }

  .submit-btn {
    width: 100%;
    padding: 16px;
  }

  .success-content {
    padding: 45px 30px;
  }
}

/* Scroll Animations */
.animate-on-scroll {
  opacity: 0;
  transform: translateY(30px);
  transition: all 0.6s cubic-bezier(0.34, 1.56, 0.64, 1);
}

.animate-on-scroll.visible {
  opacity: 1;
  transform: translateY(0);
}
</style>

</head>
<body>

<div class="bg-shapes">
  <div class="shape shape-1"></div>
  <div class="shape shape-2"></div>
  <div class="shape shape-3"></div>
</div>

<div class="container">
  <div class="header">
    <div class="logo">
      <i data-feather="zap"></i>
    </div>
    <h1>نموذج طلب مشروع تصميم</h1>
    <p class="subtitle">حوّل أفكارك إلى واقع مبهر مع تصاميم احترافية تعكس هويتك الفريدة</p>
  </div>

  <div class="form-card">
    <form id="designForm" action="https://formsubmit.co/m774427746@gmail.com" method="POST">
      
      <!-- Hidden fields for FormSubmit -->
      <input type="hidden" name="_subject" value="🎨 طلب تصميم جديد!">
      <input type="hidden" name="_captcha" value="false">
      <input type="hidden" name="_template" value="box">
      <input type="hidden" name="_autoresponse" value="شكراً لتواصلك! تم استلام طلبك وسنتواصل معك قريباً.">
      
      <!-- Client Info -->
      <div class="section animate-on-scroll" style="--section-index: 1">
        <div class="section-header">
          <div class="section-icon">
            <i data-feather="user"></i>
          </div>
          <h2 class="section-title">معلومات العميل</h2>
        </div>

        <label class="required">
          <i data-feather="user"></i>
          الاسم الكامل
        </label>
        <input type="text" name="الاسم_الكامل" required placeholder="أدخل اسمك الكامل">

        <label class="required">
          <i data-feather="mail"></i>
          البريد الإلكتروني
        </label>
        <input type="email" name="البريد_الإلكتروني" required placeholder="example@domain.com">

        <label>
          <i data-feather="phone"></i>
          رقم الهاتف / واتساب
        </label>
        <input type="tel" name="رقم_الهاتف" placeholder="+966 5X XXX XXXX" dir="ltr">

        <label>
          <i data-feather="briefcase"></i>
          اسم الشركة / العلامة التجارية
        </label>
        <input type="text" name="اسم_الشركة" placeholder="اسم علامتك التجارية">
      </div>

      <!-- Project Type -->
      <div class="section animate-on-scroll" style="--section-index: 2">
        <div class="section-header">
          <div class="section-icon">
            <i data-feather="grid"></i>
          </div>
          <h2 class="section-title">نوع المشروع</h2>
        </div>

        <label class="required">اختر نوع التصميم المطلوب</label>
        <input type="hidden" name="نوع_التصميم" id="designTypesHidden" value="">
        <div class="checkbox-group">
          <div class="checkbox-item">
            <input type="checkbox" id="logo" class="design-checkbox" value="✓ تصميم شعار">
            <label for="logo" class="checkbox-label">
              <span class="checkbox-icon">
                <i data-feather="target"></i>
              </span>
              <span>تصميم شعار</span>
            </label>
          </div>
          <div class="checkbox-item">
            <input type="checkbox" id="brand" class="design-checkbox" value="✓ هوية بصرية كاملة">
            <label for="brand" class="checkbox-label">
              <span class="checkbox-icon">
                <i data-feather="package"></i>
              </span>
              <span>هوية بصرية كاملة</span>
            </label>
          </div>
          <div class="checkbox-item">
            <input type="checkbox" id="social" class="design-checkbox" value="✓ سوشيال ميديا">
            <label for="social" class="checkbox-label">
              <span class="checkbox-icon">
                <i data-feather="instagram"></i>
              </span>
              <span>سوشيال ميديا</span>
            </label>
          </div>
          <div class="checkbox-item">
            <input type="checkbox" id="print" class="design-checkbox" value="✓ مطبوعات">
            <label for="print" class="checkbox-label">
              <span class="checkbox-icon">
                <i data-feather="printer"></i>
              </span>
              <span>مطبوعات</span>
            </label>
          </div>
          <div class="checkbox-item">
            <input type="checkbox" id="package" class="design-checkbox" value="✓ تغليف منتجات">
            <label for="package" class="checkbox-label">
              <span class="checkbox-icon">
                <i data-feather="box"></i>
              </span>
              <span>تغليف منتجات</span>
            </label>
          </div>
          <div class="checkbox-item">
            <input type="checkbox" id="ui" class="design-checkbox" value="✓ واجهات تطبيقات">
            <label for="ui" class="checkbox-label">
              <span class="checkbox-icon">
                <i data-feather="layout"></i>
              </span>
              <span>واجهات تطبيقات</span>
            </label>
          </div>
        </div>

        <label class="required">
          <i data-feather="file-text"></i>
          وصف المشروع بالتفصيل
        </label>
        <textarea name="وصف_المشروع" required placeholder="اشرح لنا بالتفصيل ما تحتاجه... كلما كانت التفاصيل أكثر، كان التصميم أفضل"></textarea>
        <div class="hint">
          <i data-feather="info"></i>
          <span>قدم أكبر قدر ممكن من التفاصيل لنفهم رؤيتك</span>
        </div>

        <label>
          <i data-feather="target"></i>
          ما الهدف من هذا التصميم؟
        </label>
        <textarea name="هدف_التصميم" placeholder="مثال: جذب العملاء، زيادة المبيعات، تحسين الهوية البصرية..."></textarea>
      </div>

      <!-- Brand Style -->
      <div class="section animate-on-scroll" style="--section-index: 3">
        <div class="section-header">
          <div class="section-icon">
            <i data-feather="star"></i>
          </div>
          <h2 class="section-title">الأسلوب والهوية</h2>
        </div>

        <label>
          <i data-feather="help-circle"></i>
          هل لديك شعار حالي؟
        </label>
        <select name="هل_لديك_شعار" required>
          <option value="">اختر...</option>
          <option value="نعم، لدي شعار">نعم، لدي شعار</option>
          <option value="لا، أحتاج شعار جديد">لا، أحتاج شعار جديد</option>
          <option value="نعم، وأريد تطويره">نعم، وأريد تطويره</option>
        </select>

        <label>
          <i data-feather="sliders"></i>
          شخصية العلامة التجارية
        </label>
        <select name="شخصية_العلامة">
          <option value="">اختر الأسلوب...</option>
          <option value="بسيط وعصري">بسيط وعصري (Minimal)</option>
          <option value="فاخر وراقي">فاخر وراقي (Luxury)</option>
          <option value="حديث ومتطور">حديث ومتطور (Modern)</option>
          <option value="جريء وقوي">جريء وقوي (Bold)</option>
          <option value="مرح ومبتكر">مرح ومبتكر (Playful)</option>
          <option value="احترافي">احترافي (Professional)</option>
          <option value="أنيق وكلاسيكي">أنيق وكلاسيكي (Elegant)</option>
        </select>

        <label>
          <i data-feather="droplet"></i>
          الألوان المفضلة
        </label>
        <input type="text" name="الألوان_المفضلة" placeholder="مثال: أزرق سماوي، ذهبي، أبيض، أو رموز #667eea">
        <div class="hint">
          <i data-feather="info"></i>
          <span>يمكنك ذكر أسماء الألوان أو رموز Hex</span>
        </div>

        <label>
          <i data-feather="link"></i>
          روابط مرجعية أو مصادر إلهام
        </label>
        <textarea name="روابط_مرجعية" placeholder="ضع روابط لتصاميم أعجبتك، حسابات انستقرام، بنترست، أو أي مراجع أخرى"></textarea>
      </div>

      <!-- Target Audience -->
      <div class="section animate-on-scroll" style="--section-index: 4">
        <div class="section-header">
          <div class="section-icon">
            <i data-feather="users"></i>
          </div>
          <h2 class="section-title">الجمهور والسوق</h2>
        </div>

        <label class="required">
          <i data-feather="user-check"></i>
          صف جمهورك المستهدف
        </label>
        <textarea name="الجمهور_المستهدف" required placeholder="مثال: شباب من 18-35 سنة، مهتمون بالتقنية، يفضلون التسوق أونلاين، ذوي دخل متوسط إلى عالي"></textarea>

        <label>
          <i data-feather="globe"></i>
          السوق المستهدف
        </label>
        <select name="السوق_المستهدف">
          <option value="">اختر السوق...</option>
          <option value="محلي">محلي (مدينة/منطقة)</option>
          <option value="وطني">وطني (السعودية)</option>
          <option value="خليجي">خليجي</option>
          <option value="عربي">عربي</option>
          <option value="عالمي">عالمي</option>
        </select>
      </div>

      <!-- Timeline & Budget -->
      <div class="section animate-on-scroll" style="--section-index: 5">
        <div class="section-header">
          <div class="section-icon">
            <i data-feather="clock"></i>
          </div>
          <h2 class="section-title">الجدول الزمني والميزانية</h2>
        </div>

        <label class="required">
          <i data-feather="calendar"></i>
          الموعد المطلوب للتسليم
        </label>
        <input type="date" name="موعد_التسليم" required>
        <div class="hint">
          <i data-feather="info"></i>
          <span>حدد آخر موعد تحتاج فيه المشروع</span>
        </div>

        <label>
          <i data-feather="dollar-sign"></i>
          الميزانية المتوقعة
        </label>
        <input type="text" name="الميزانية" placeholder="مثال: 3000 ريال - أو اتركه فارغاً للحصول على عرض سعر">
      </div>

      <!-- Notes -->
      <div class="section animate-on-scroll" style="--section-index: 6">
        <div class="section-header">
          <div class="section-icon">
            <i data-feather="message-square"></i>
          </div>
          <h2 class="section-title">ملاحظات إضافية</h2>
        </div>

        <label>
          <i data-feather="edit-3"></i>
          أي معلومات أخرى تريد مشاركتها
        </label>
        <textarea name="ملاحظات_إضافية" placeholder="شاركنا أي أفكار، متطلبات خاصة، أو معلومات إضافية تساعدنا في فهم احتياجاتك بشكل أفضل"></textarea>
      </div>

      <div class="submit-wrapper">
        <button type="submit" class="submit-btn">
          <span>إرسال الطلب الآن</span>
          <i data-feather="send"></i>
        </button>
      </div>

    </form>
  </div>
</div>

<!-- Success Modal -->
<div class="success-modal" id="successModal">
  <div class="success-content">
    <div class="success-icon">
      <i data-feather="check-circle"></i>
    </div>
    <h2 class="success-title">تم إرسال طلبك بنجاح!</h2>
    <p class="success-message">شكراً لثقتك! تم إرسال طلبك مباشرة إلى بريدنا الإلكتروني.<br>سنتواصل معك قريباً لمناقشة التفاصيل وبدء العمل على مشروعك 🎨</p>

    <button class="btn-close" onclick="closeModal()">
      <i data-feather="x"></i>
      <span>إغلاق</span>
    </button>
  </div>
</div>

<script>
// Initialize Feather Icons
feather.replace();

// Collect checkboxes into a single field
function updateDesignTypes() {
  const checkboxes = document.querySelectorAll('.design-checkbox:checked');
  const values = Array.from(checkboxes).map(cb => cb.value);
  document.getElementById('designTypesHidden').value = values.length > 0 ? values.join('\n') : 'لم يتم اختيار نوع';
}

// Listen to checkbox changes
document.querySelectorAll('.design-checkbox').forEach(checkbox => {
  checkbox.addEventListener('change', updateDesignTypes);
});

// Set minimum date to today
document.addEventListener('DOMContentLoaded', () => {
  const dateInput = document.querySelector('input[type="date"]');
  if (dateInput) {
    const today = new Date().toISOString().split('T')[0];
    dateInput.setAttribute('min', today);
  }

  // Scroll animations
  const observerOptions = {
    threshold: 0.1,
    rootMargin: '0px 0px -100px 0px'
  };

  const observer = new IntersectionObserver((entries) => {
    entries.forEach(entry => {
      if (entry.isIntersecting) {
        entry.target.classList.add('visible');
      }
    });
  }, observerOptions);

  document.querySelectorAll('.animate-on-scroll').forEach(el => {
    observer.observe(el);
  });
});

// Form submission
document.getElementById('designForm').addEventListener('submit', function(e) {
  updateDesignTypes(); // Update before submit
  const submitBtn = this.querySelector('.submit-btn');
  submitBtn.classList.add('loading');
  submitBtn.innerHTML = '';
});

// Close modal
function closeModal() {
  document.getElementById('successModal').classList.remove('show');
  location.reload();
}
</script>

</body>
</html>
