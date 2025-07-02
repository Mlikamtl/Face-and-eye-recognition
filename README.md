
# 👁️ تشخیص چهره و چشم با OpenCV

پروژه‌ای ساده و آموزشی برای تشخیص چهره و چشم با استفاده از **OpenCV** و **مدل‌های پیش‌آموزش‌دیده Haar Cascade**. این پروژه به صورت زنده از طریق وب‌کم تصویر می‌گیرد و همچنین روی یک تصویر ذخیره‌شده نیز پردازش انجام می‌دهد.

## 🧠 ویژگی‌ها

* تشخیص چهره با استفاده از `haarcascade_frontalface_default.xml`
* تشخیص چشم با استفاده از `haarcascade_eye.xml`
* نمایش تصاویر ورودی، خاکستری، و نتایج تشخیص با کادر
* پشتیبانی از تصویر ثابت و تصویر زنده وب‌کم

## 🖼️ پیش‌نمایش

<p align="center">
  <img src="preview.gif" alt="Face Detection Preview" width="600"/>
</p>

## 🛠️ نصب پیش‌نیازها

```bash
pip install opencv-python matplotlib
```

> توجه: اگر از Jupyter Notebook استفاده می‌کنید، ممکن است نیاز به فعال‌سازی `%matplotlib widget` داشته باشید.

## 📂 ساختار فایل‌ها

```
├── haarcascade_frontalface_default.xml
├── haarcascade_eye.xml
├── mlika4.jpg
├── face_eye_detection.py
└── README.md
```

## ▶️ اجرای کد

```bash
python face_eye_detection.py
```

یا اگر در Jupyter Notebook هستید:

```python
%matplotlib widget
```

## 📸 توضیح عملکرد کد

1. بارگذاری تصویر `mlika4.jpg`
2. گرفتن تصویر از وب‌کم و نمایش آن
3. بارگذاری مدل‌های Haar برای تشخیص چهره و چشم
4. تبدیل تصویر به حالت خاکستری
5. انجام عملیات تشخیص
6. کشیدن مستطیل دور چهره‌ها و چشم‌ها
7. نمایش نتایج با OpenCV

## ⚠️ نکات مهم

* فایل‌های مدل باید در مسیر پروژه وجود داشته باشند.
* استفاده از `cv2.imshow` در محیط‌هایی مثل Jupyter ممکن است مشکل داشته باشد. در این صورت از `matplotlib` استفاده کنید.

## 📌 TODOهای پیشنهادی برای ارتقاء

* افزودن قابلیت تشخیص چند چهره به‌طور همزمان
* ذخیره‌سازی نتایج در فایل خروجی
* اضافه‌کردن مدل‌های دقیق‌تر مثل DNN یا MTCNN

* 


👁️ Face and Eye Detection with OpenCV

A simple and educational project to detect **faces and eyes** using **OpenCV** and **pre-trained Haar Cascade models**. This script processes both a static image and a live webcam feed, drawing bounding boxes around detected features.

🧠 Features

* Face detection using `haarcascade_frontalface_default.xml`
* Eye detection using `haarcascade_eye.xml`
* Displays original, grayscale, and detection results
* Supports both static image and live webcam input

 🖼️ Preview

<p align="center">
  <img src="preview.gif" alt="Face Detection Preview" width="600"/>
</p>

 🛠️ Requirements

Install the required libraries:

```bash
pip install opencv-python matplotlib
```

> Note: If you're using Jupyter Notebook, enable interactive mode with `%matplotlib widget`.

📂 File Structure

```
├── haarcascade_frontalface_default.xml
├── haarcascade_eye.xml
├── mlika4.jpg
├── face_eye_detection.py
└── README.md
```

 ▶️ How to Run

Run the Python script:

```bash
python face_eye_detection.py
```

Or inside a Jupyter Notebook:

```python
%matplotlib widget
```

 📸 How It Works

1. Loads an image (`mlika4.jpg`)
2. Captures an image from the webcam and displays it
3. Loads Haar Cascade models for face and eye detection
4. Converts the image to grayscale
5. Performs face and eye detection
6. Draws bounding boxes on detected features
7. Displays the results using OpenCV

 ⚠️ Notes

* Make sure the Haar cascade XML files are present in your project directory.
* `cv2.imshow()` might not work properly in Jupyter; you can use `matplotlib` instead if needed.

 🚀 Future Improvements

* Add support for detecting multiple faces at once
* Save output image to file
* Use more advanced models like DNN or MTCNN for better accuracy

