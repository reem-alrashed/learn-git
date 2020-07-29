<div dir="rtl" align="right">

## الدمج بين التفرعات - (branches merge):
يستخدم هذا الأمر  لدمج تفرعين أو أكثر للتطور معًا. 
أولاً على سبيل المثال تفقد التفرعات الموجودة على المستودع
<div dir="ltr" align="left">

```git 
	git branch
```

</div>
ستكون المخرجات الفرع الأساسي (`master*`) فقط في حال عدم انشاء تفرعات أخرى. 
  
  وعلامة النجمة تعني بأنه الفرع الذي تعمل به حالياً

 الآن لإنشاء فرع جديد:
 <div dir="ltr" align="left">   
 
 ```git 
 	git branch my-branch
```

 </div>
  وبالتالي تكون قد أنشأت نسخة لجميع الملفات الموجودة في الفرع الأصلي master. لتنتقل الآن لفرع الجديد الذي أنشأته

 <div dir="ltr" align="left">
 
```git 
	git checkout my-branch
```

</div>

 لإظهار الأفرع الموجودة حالياً
<div dir="ltr" align="left">

```git 
	git branch
```

</div>

ستكون المخرجات:   

master   

my-branch*

</div>
