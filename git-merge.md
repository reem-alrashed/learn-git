<div dir="rtl" align="right">
	
## الدمج بين التفرعات branches merge
يستخدم هذا الأمر  لدمج تفرعين أو أكثر للتطور معًا. 
أولاً على سبيل المثال تفقد التفرعات الموجودة على المستودع
<div dir="ltr" align="left">

```git 
	git branch
```

</div>
ستكون المخرجات الفرع الأساسي `master*` فقط في حال عدم انشاء تفرعات أخرى. 
  
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
<div dir="ltr" align="left">
	
```
master   

my-branch*  

```

</div>
كما تلاحظ فقد عرض لنا فرعين، والنجمة موضوعة على الفرع الجديد أي أنك الآن ضمنه.

الآن يمكنك إجراء التغييرات التي تريد وكيفما تريد دون قلق فأنت الآن ضمن فرع مستقل ولن تُحدث مشاكل في الفرع الأساسي.
بعد انتهاءك من العمل على الفرع الجديد، يمكنك الانتقال للفرع الأصلي ودمج التغييرات
    
<div dir="ltr" align="left">  
	
```git	
 git checkout master
 git branch
```
<div dir="rtl" align="right">
 المخرجات:
</div>

```
master*
my-branch
```

</div>
هنا انتقلنا للفرع الأساسي master وتأكدنا بوجود النجمة بجواره أي أننا فعلاً ضمنه الآن. لدمج. 

<div dir="ltr" align="left">
	
```
git merge my-branch
```

</div>

وبهذا تم دمج الكود في الفرع الذي أنشأته my-branch مع الكود الأصلي في التفرع master.

</div>
