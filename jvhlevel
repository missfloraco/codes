// منع نسخ محتوى الموقع ----------------------------------------------------------------------------------------

<script>
  // منع الضغط بزر الفأرة الأيمن
  document.addEventListener("contextmenu", function(event) {
    event.preventDefault();
  });

  // تعطيل اختصارات لوحة المفاتيح
  document.addEventListener("keydown", function(event) {
    // F12، Ctrl+Shift+I، Ctrl+Shift+J، Ctrl+Shift+C، Ctrl+U
    if (
      event.key === "F12" || // F12
      (event.ctrlKey && event.shiftKey && ["I", "J", "C"].includes(event.key.toUpperCase())) || 
      (event.ctrlKey && event.key.toUpperCase() === "U") // Ctrl+U
    ) {
      event.preventDefault();
      event.stopPropagation();
    }
  });

  // تعطيل النسخ وتحديد النص
  document.addEventListener("copy", function(event) {
    event.preventDefault();
  });
  
  document.addEventListener("cut", function(event) {
    event.preventDefault();
  });

  document.addEventListener("selectstart", function(event) {
    event.preventDefault();
  });

  // تعطيل خاصية الفحص باستخدام Ctrl+Shift+I بشكل أعمق
  document.onkeydown = function(event) {
    if (
      (event.ctrlKey && event.shiftKey && event.keyCode === 73) || // Ctrl+Shift+I
      (event.ctrlKey && event.shiftKey && event.keyCode === 74) || // Ctrl+Shift+J
      (event.ctrlKey && event.keyCode === 85) || // Ctrl+U
      (event.keyCode === 123) // F12
    ) {
      return false;
    }
  };

  // تعطيل سحب العناصر على الصفحة
  document.addEventListener("dragstart", function(event) {
    event.preventDefault();
  });
</script>
