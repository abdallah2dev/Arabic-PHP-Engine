<div dir="rtl">

# مكتبة البي اتش بي العربي ع

مكتبة البي اتش بي العربي تضم مجموعة ضخمة من العمليات باللغة العربية ومحرك لقالب PHP ليتمكن المطور من كتابة أكواد PHP باللغة العربية.

كتبت باللغة العربية لتسهيل تطوير المواقع للمطورين العرب.

بإمكان المطور كتابة أكواد PHP باللغة العربية أو اللغة الإنكليزية ضمن القالب.

يسهل القالب عمل المطور حيث يتم كتابة أكواد و عمليات PHP جنباً إلى جنب مع أكواد HTML.

يمكن استخدام المكتبة بعد تضمين الملف الخاص بها كما يلي:

```php
require_once 'Arabic-PHP-Engine.php';
```

يمكنك استخدام القالب لتضمين الملفات كم يلي:

```php
$ع = new ع;
$ع->تضمين( رابط الملف 1 );
$ع->تضمين( رابط الملف 2 );
$ع->تضمين( رابط الملف 3 );
```

**ما يمكن كتابته باللغة العربية ضمن القالب**

```php
؛   -   ;
،   -   ,
ع.إذا_كان   -   if
ع.أو_إذا   -   else if
ع.آخر   -   else
ع.عملية   -   function
ع.سويتش   -   switch
ع.الحالة   -   case
ع.إفتراضي   -   default
ع.بينما   -   while
ع.عمل   -   do
ع.من_أجل   -   for
ع.من_أجل_الكل   -   foreach
ع.مصفوفة   -   array
ع.كـ   -   as
ع.عام   -   global
```

**مثال**

```html
<div>سطر 1</div>
<div>سطر 2</div>
ع_ع
$تم_الدخول = خاطئ؛
ع.إذا_كان( $تم_الدخول ){
ع_ع
<span>تم تسجيل الدخول</span>
ع_ع
}ع.آخر{
ع_ع
<span>فضلاً قم بتسجيل الدخول</span>
ع_ع
}
ع_ع
```

بداية ونهاية الكود الأساسية هي "ع_ع"

يمكن تغيير البداية والنهاية لنص مخصص عن طريق الكود التالي:

```php
$ع->الرمز = "النص";
```

يمكنك استخدام أكواد PHP الأساسية ضمن القالب بدون أخطاء إذا احتجت إلى ذلك.


# العمليات والمتغيرات باللغة العربية

### المتغيرات

يمكن استخدامها ضمن القالب أو خارجه بدون مشاكل

- **لغة_المتصفح:** اللغة الحالية للمتصفح من حرفين ar , en ...
```php
طباعة( لغة_المتصفح );
النتيجة: نص من حرفين
```

- **اسم_الملف_الحالي:** اسم الملف الحالي PHP_SELF
```php
طباعة( اسم_الملف_الحالي );
النتيجة: نص
```

- **ايبي_المضيف:** اي بي المضيف SERVER_ADDR
```php
طباعة( ايبي_المضيف );
النتيجة: نص
```
- **نوع_الطلب:** نوع طلب الصفحة post , get
```php
طباعة( نوع_الطلب );
النتيجة: نص
```

- **متغيرات_الرابط:** ?id=1&name=test...
```php
طباعة( متغيرات_الرابط );
النتيجة: نص
```

- **الدومين:** دومين الموقع
```php
طباعة( الدومين );
النتيجة: نص
```

- **ايبي_المستخدم:** اي بي المستخدم REMOTE_ADDR
```php
طباعة( ايبي_المستخدم );
النتيجة: نص
```

- **رابط_الملف_الكامل:** الرابط الكامل للملف SCRIPT_FILENAME
```php
طباعة( رابط_الملف_الكامل );
النتيجة: نص
```

- **فروع_الرابط:** فروع الرابط /blog/year/month/day/
```php
طباعة( فروع_الرابط );
النتيجة: مصفوفة تحوي كل الفروع
```

- **صحيح:** تستخدم في أي مكان بدل true
```php
$متغير = صحيح;
```

- **خاطئ:** تستخدم في أي مكان بدل false
```php
$متغير = خاطئ;
```

- **الأمان_مفعل:** إذا كان التصفح عبر https
```php
طباعة( الأمان_مفعل );
النتيجة: true أو false
```

- **الرابط_الأساسي:** رابط الموقع الأساسي بدون فروع أو متغيرات http://www.example.com/
```php
طباعة( الرابط_الأساسي );
النتيجة: نص
```

- **الرابط_الكامل:**الرابط الكامل للصفحة http://www.example.com/blog/year/month/day/name
```php
طباعة( الرابط_الكامل );
النتيجة: نص
```

- **معرف_المتصفح:** معرف المتصفح user agent
```php
طباعة( معرف_المتصفح );
النتيجة: نص
```

- **هل_التصفح_من_هاتف:** إذا كان التصفح عبر هاتف
```php
طباعة( هل_التصفح_من_هاتف );
النتيجة: true أو false
```

### العمليات العامة

- **توليد_نص():** توليد نص عشوائي
```php
توليد_نص( [$الحجم] );
$الحجم = 10
النتيجة: نص
```

- **توليد_رقم():** توليد رقم عشوائي
```php
توليد_رقم( [$الحجم] );
$الحجم = 10
النتيجة: نص
```

- **ايقاف_السكربت_مؤقت()** - إيقاف السكربت وقت محدد sleep
```php
ايقاف_السكربت_مؤقت( $الوقت );
```

- **ايقاف_السكربت()** - إيقاف السكربت ومنع متابعة استخراجه
```php
ايقاف_السكربت();
```

- **تصمين_ملف()** - لتضمين ملف داخل السكربت include
```php
تصمين_ملف( $الملف );
```

- **تعريف_متغير()** - تعريف متغير لتتمكن من استخدامه ضمن السكربت في أي مكان define
```php
تعريف_متغير( $الاسم , $المتفير );
```

- **هل_المتغير_بريد()** - إذا كان المتغير بريد إلكتروني
```php
هل_المتغير_بريد( $المتفير );
النتيجة: true أو false
```

- **هل_المتغير_بلا_قيمة()** - إذا كان المتغير له قيمة empty
```php
هل_المتغير_بلا_قيمة( $المتفير );
النتيجة: true أو false
```

- **جلب_الرقم()** - استخراج الرقم من النص intval
```php
جلب_الرقم( $النص );
النتيجة: رقم
```

- **جلب_الرقم_مع_فواصل()** - استخراج الرقم مع الفواصل من النص floatval
```php
جلب_الرقم_مع_فواصل( $النص );
النتيجة: رقم
```

- **طباعة_مصفوفة()** - طباعة مصفوفة print_r
```php
طباعة_مصفوفة( $المصفوفة );
```

- **طباعة()** - طباعة نص echo
```php
طباعة( $النص );
```

- **هل_رابط_الإحالة_معرف()** - هل الرابط مباشر أو تم التحويل من رابط آخر $_SERVER["HTTP_REFERER"]
```php
هل_رابط_الإحالة_معرف();
النتيجة: true أو false
```

- **جلب_مصفوفة_الفروع()** - جلب فروع الرابط 
```php
جلب_مصفوفة_الفروع( $مجلد_الموقع = "" );
النتيجة: مصفوفة

http://example.com/blog/year/month/day
جلب_مصفوفة_الفروع();
النتيجة: array( 0 => "blog" , 1 => "year" , 2 => "month" , 3 => "day" )

http://example.com/blog/year/month/day
جلب_مصفوفة_الفروع( "blog" );
جلب_مصفوفة_الفروع( "blog/" );
النتيجة: array( 0 => "year" , 1 => "month" , 2 => "day" )
```

### عمليات المصفوفة array

- **تغيير_حالة_أحرف_المصفوفة()** - تغيير حالة أحرف مفاتيح المصفوفة array_change_key_case
```php
تغيير_حالة_أحرف_المصفوفة( $المصفوفة , أحرف_كبيرة | أحرف_صغيرة );
النتيجة: مصفوفة
```

- **تقسيم_المصفوفة()** - تقسيم المصفوفة إلى مصفوفات ضمن المصفوفة الأساسية array_chunk
```js
تقسيم_المصفوفة( $المصفوفة , $العدد );
النتيجة: مصفوفة
```

- **دمج_مصفوفتين()** - دمج مصفوفتين الأولى تكون مفاتيح والثانية قيم array_combine
```js
دمج_مصفوفتين( $المصفوفة_1 , $المصفوفة_2 );
النتيجة: مصفوفة
```

- **فرق_القيم_بين_المصفوفات()** - ايجاد الفرق بين المصفوفات array_diff
```php
فرق_القيم_بين_المصفوفات( $المصفوفة1 [, $المصفوفة2] [, $المصفوفة3] -. )
النتيجة: مصفوفة
```

- **قلب_القيم_والمفاتيح_للمصفوفة()** - التبديل بين القيم و المفاتيح للمصفوفة array_flip
```php
قلب_القيم_والمفاتيح_للمصفوفة( $المصفوفة );
النتيجة: مصفوفة
```

- **ايجاد_القيم_المشتركة_بين_المصفوفات()** - ايجاد القيم المشتركة بين المصفوفات array_intersect
```php
ايجاد_القيم_المشتركة_بين_المصفوفات( $المصفوفة1 [, $المصفوفة2] [, $المصفوفة3] ... );
النتيجة: مصفوفة
```

- **هل_تحوي_المصفوفة_مفتاح()** - إذا كانت المصفوفة تحوي مفتاح array_key_exists
```php
هل_تحوي_المصفوفة_مفتاح( $المفتاح , $المصفوفة );
النتيجة: true أو false
```

- **جلب_مفاتيح_المصفوفة()** - جلب مفاتيح المصفوفة ضمن مصفوفة جديدة array_keys
```php
جلب_مفاتيح_المصفوفة( $المصفوفة );
النتيجة: مصفوفة
```

- **تطبيق_عملية_على_قيم_المصفوفة()** - تطبيق عملية محددة على كافة قيم المصفوفة array_map
```php
تطبيق_عملية_على_قيم_المصفوفة( $المصفوفة1 [, $المصفوفة2] [, $المصفوفة3] ... );
```

- **دمج_مصفوفات()** - دمج عدة مصفوفات array_merge
```php
دمج_مصفوفات( $المصفوفة1 [, $المصفوفة2] [, $المصفوفة3] ... );
النتيجة: مصفوفة
```

- **حذف_آخر_عنصر_من_المصفوفة()** - حذف آخر عنصر من المصفوفة array_pop
```php
حذف_آخر_عنصر_من_المصفوفة( $المصفوفة );
```

- **إضافة_عناصر_إلى_المصفوفة()** - إضافة قيم إلى نهاية المصفوفة array_push
```php
إضافة_عناصر_إلى_المصفوفة( $المصفوفة , $القيمة1 [, $القيمة2] [, $القيمة3 ] ... );
```

- **جلب_عناصر_عشوائية_من_المصفوفة()** - جلب عناصر عشوائية من المصفوفة array_rand
```php
جلب_عناصر_عشوائية_من_المصفوفة( $المصفوفة , $العدد );
النتيجة: مصفوفة
```

- **عكس_المصفوفة()** - عكس المصفوفة array_reverse
```php
عكس_المصفوفة( $المصفوفة );
النتيجة: مصفوفة
```

- **بحث_في_المصفوفة()** - بحث عن قيمة ضمن المصفوفة و إرجاع المفتاح array_search
```php
بحث_في_المصفوفة( $البحث , $المصفوفة );
النتيجة: نص
```

- **حذف_أول_عنصر_من_المصفوفة()** - حذف أول عنصر من المصفوفة array_shift
```php
حذف_أول_عنصر_من_المصفوفة( $المصفوفة );
```

- **جلب_قسم_من_المصفوفة()** - جلب قسم من المصفوفة ضمن مصفوفة جديدة array_slice
```php
جلب_قسم_من_المصفوفة( $المصفوفة , $البداية [, $الحجم] );
النتيجة: مصفوفة
```

- **جلب_مجموع_قيم_المصفوفة()** - جلب مجموع قيم المصفوفة الرقمية array_sum
```php
جلب_مجموع_قيم_المصفوفة( $المصفوفة );
النتيجة: رقم
```

- **حذف_المكرر_من_المصفوفة()** - حذف القيم المكررة من المصفوفة array_unique
```php
حذف_المكرر_من_المصفوفة( $المصفوفة );
النتيجة: مصفوفة
```

- **إضافة_عناصر_إلى_بداية_المصفوفة()** - إضافة قيم إلى بداية المصفوفة array_unshift
```php
إضافة_عناصر_إلى_بداية_المصفوفة( $المصفوفة , $القيمة1 [, $القيمة2] [, $القيمة3 ] ... );
```

- **جلب_قيم_المصفوفة()** - جلب قيم المصفوفة فقط ضمن مصفوفة جديدة array_values
```php
جلب_قيم_المصفوفة( $المصفوفة );
النتيجة: مصفوفة
```

- **ترتيب_قيم_المصفوفة_تصاعدي()** - ترتيب المصفوفة تصاعدياً حسب القيم asort
```php
ترتيب_قيم_المصفوفة_تصاعدي( $المصفوفة );
النتيجة: مصفوفة
```

- **ترتيب_قيم_المصفوفة_تنازلي()** - ترتيب المصفوفة تنازلياً حسب القيم arsort
```php
ترتيب_قيم_المصفوفة_تنازلي( $المصفوفة );
النتيجة: مصفوفة
```

- **حجم_المصفوفة()** - جلب عدد عناصر المصفوفة count
```php
حجم_المصفوفة( $المصفوفة );
النتيجة: رقم
```

- **جلب_العنصر_الحالي_للمصفوفة()** - جلب العنصر الحالي من المصفوفة current
```php
جلب_العنصر_الحالي_للمصفوفة( $المصفوفة );
```

- **جلب_العنصر_الأول_للمصفوفة()** - جلب العنصر الأول من المصفوفة reset
```php
جلب_العنصر_الأول_للمصفوفة( $المصفوفة );
```

- **جلب_العنصر_الأخير_للمصفوفة()** - جلب العنصر الأخير من المصفوفة end
```php
جلب_العنصر_الأخير_للمصفوفة( $المصفوفة );
```

- **جلب_العنصر_التالي_للمصفوفة()** - جلب العنصر التالي من المصفوفة next
```php
جلب_العنصر_التالي_للمصفوفة( $المصفوفة );
```

- **جلب_العنصر_السابق_للمصفوفة()** - جلب العنصر السابق من المصفوفة prev
```php
جلب_العنصر_السابق_للمصفوفة( $المصفوفة );
```

- **ترتيب_مفاتيح_المصفوفة_تصاعدي()** - ترتيب المصفوفة تصاعدياً حسب المفاتيح ksort
```php
ترتيب_مفاتيح_المصفوفة_تصاعدي( $المصفوفة );
النتيجة: مصفوفة
```

- **ترتيب_مفاتيح_المصفوفة_تنازلي()** - ترتيب المصفوفة تنازلياً حسب المفاتيح krsort
```php
ترتيب_مفاتيح_المصفوفة_تنازلي( $المصفوفة );
النتيجة: مصفوفة
```

- **توليد_مصفوفة_أرقام()** - توليد مصفوفة من أرقام range
```php
توليد_مصفوفة_أرقام( $الرقم_الأصغر , $الرقم_الأكبر [, $الفاصل_بين_الأرقام] );
$الفاصل_بين_الأرقام = 1 
النتيجة: مصفوفة
```

- **ترتيب_المصفوفة_عشوائي()** - ترتيب المصفوفة بشكل عشوائي shuffle
```php
ترتيب_المصفوفة_عشوائي( $المصفوفة );
النتيجة: مصفوفة
```

- **ترتيب_المصفوفة_تصاعدي()** - ترتيب المصفوفة تصاعدياً sort
```php
ترتيب_المصفوفة_تصاعدي( $المصفوفة );
النتيجة: مصفوفة
```

- **ترتيب_المصفوفة_تنازلي()** - ترتيب المصفوفة تنازلياً rsort
```php
ترتيب_المصفوفة_تنازلي( $المصفوفة );
النتيجة: مصفوفة
```

- **هل_تملك_المصفوفة_عنصر()** - إذا كانت المصفوفة تحوي قيمة in_array
```php
هل_تملك_المصفوفة_عنصر( $البحث , $المصفوفة );
النتيجة: true أو false
```

- **هل_المصفوفة_تحوي_مفاتيح()** - إذا كانت المصفوفة تحوي مفاتيح
```php
هل_المصفوفة_تحوي_مفاتيح( $المصفوفة );
["blue","red"] خاطئ
["a"=>"blue","b"=>"red"] صحيح
النتيجة: true أو false
```

- **كل()** - لتنفيذ عملية على مفاتيح وقيم المصفوفة
```php
كل( $المصفوفة , function( $المفتاح , $القيمة ){  } );
يمكن استخدامها مع المصفوفة التي تحوي مفاتيح
أو مع المصفوفة بدون مفاتيح وتكون قيمة المقتاح هي موضع العنصر
```

### عمليات الوقت

- **عدد_أيام_الشهر()** - جلب عدد أيام الشهر من السنة
```php
عدد_أيام_الشهر( $الشهر , $السنة );
النتيجة: رقم
```

- **جلب_المنطقة_الزمنية()** - جلب المنطقة الزمنية الحالية
```php
جلب_المنطقة_الزمنية();
النتيجة: نص
```

- **تغيير_المنطقة_الزمنية()** - تغيير المنطقة الزمنية الحالية
```php
تغيير_المنطقة_الزمنية( $المنطقة_الزمنية );
```

- **الوقت()** - العملية تغنيك عن استخدام time , date
```php
الوقت(); إرجاع تايم ستامب
الوقت( $المطلوب ); إرجاع قيمة المطلوب يوم، شهر، سنة -.
الوقت( "صيغة" ); إرجاع نص بالقيم المطلوبة
مثال الوقت( "س-ر-م ع:د:ث و" );
س   -   سنة
ش   -   اسم الشهر
ر   -   رقم الشهر
ي   -   اسم اليوم
م   -   رقم اليوم
ع   -   الساعة 12
ة   -   الساعة 24
د   -   دقيقة
ث   -   ثانية
و   -   الوضع مساءً أو صباحاً
```

- **النص_إلى_وقت()** - تحويل النص إلى وقت تايم ستامب strtotime
```php
النص_إلى_وقت( $النص );
النتيجة: رقم
```

### عمليات النصوص

- **اقتطاع()** - اقتطاع جزء محدد من النص mb_substr
```php
اقتطاع( $النص , $البداية [, $الحجم]  );
النتيجة: نص
```

- **استبدال_الكل()** - البحث عن كل النصوص المطابقة واستبدالها str_replace
```php
استبدال_الكل( $النص , $البحث , $الاستبدال );
النتيجة: نص
```

- **استبدال()** - البحث عن نص واستبداله بآخر مرة واحدة preg_replace
```php
استبدال( $النص , $البحث , $الاستبدال );
النتيجة: نص
```

- **إضافة_سلاش()** - إضافة سلاش إلى علامات التنصيص addslashes
```php
إضافة_سلاش( $النص );
النتيجة: نص
```

- **حذف_سلاش()** - حذف جميع السلاش من النص stripslashes
```php
حذف_سلاش( $النص );
النتيجة: نص
```

- **تقطيع_النص()** - تقسيم النص إلى مصفوفة بناءً على بحث explode
```php
تقطيع_النص( $الفاصل , $النص );
النتيجة:مصفوفة
```

- **جمع_النصوص_من_مصفوفة()** - جمع قيم المصفوفة وتحويلها إلى نص implode
```php
جمع_النصوص_من_مصفوفة( $الفاصل , $المصفوفة );
النتيجة: نص
```

- **حذف_المسافات_من_يسار_النص()** - حذف المسافات من يسار النص ltrim
```php
حذف_المسافات_من_يسار_النص( $النص );
النتيجة: نص
```

- **حذف_المسافات_من_يمين_النص()** - حذف المسافات من يمين النص rtrim
```php
حذف_المسافات_من_يمين_النص( $النص );
النتيجة: نص
```

- **تشفير_ام_دي_5()** - تشفير النص وتحويله إلى md5
```php
تشفير_ام_دي_5( $النص );
النتيجة: نص
```

- **تشفير_شا_1()** - تشفير النص وتحويله إلى sha1
```php
تشفير_شا_1( $النص );
النتيجة: نص
```

- **استبدال_متغيرات_النصوص()** - 
```php
استبدال المتغيرات ضمن النص %s sprintf
```

- **عدد_الخانات()** - جلب عدد أحرف النص mb_strlen
```php
عدد_الخانات( $النص );
النتيجة: رقم
```

- **عدد_الكلمات()** - جلب عدد الكلمات ضمن النص str_word_count
```php
عدد_الكلمات( $النص );
النتيجة: رقم
```

- **عكس_النص()** - قلت أحرف النص بين بعضها strrev
```php
عكس_النص( $النص );
النتيجة: نص
```

- **موضع_النص()** - ايجاد موضع نص ضمن النص الأساسي mb_strpos
```php
موضع_النص( $النص , $البحث [, $البداية] );
النتيجة: رقم
```

- **تبديل_لكبير()** - تحويل النص إلى أحرف كبيرة strtoupper
```php
تبديل_لكبير( $النص );
النتيجة: نص
```

- **تبديل_لصغير()** - تحويل النص إلى أحرف صغيرة strtolower
```php
تبديل_لصغير( $النص );
النتيجة: نص
```

- **عدد_المطابقات()** - إيجاد عدد المطابقات ضمن النص substr_count
```php
عدد_المطابقات( $النص , المطابقة [, $البداية ][, $مجال_البحث] );
النتيجة: رقم
```

- **إضافة_نص_كل()** - إضافة نص إلى النص كل عدد أحرف معين wordwrap
```php
إضافة_نص_كل( $النص , $الحجم = 75 , $بداية_السطر = "\n" );
النتيجة: نص
```

- **الكود_إلى_نص()** - طباعة النص مع تجاهل HTML htmlspecialchars
```php
الكود_إلى_نص( $النص );
النتيجة: نص
```

### عمليات الأرقام

- **جلب_الرقم_الإيجابي()** - جلب الرقم الايجابي من الرقم المعطى abs
```php
جلب_الرقم_الإيجابي( $الرقم );
النتيجة: رقم
```

- **تقريب_لأعلى()** - تقريب الرقم للعدد الأعلى ceil
```php
تقريب_لأعلى( $الرقم );
النتيجة: رقم
```

- **تقريب_لأسفل()** - تقريب الرقم للعدد الأدنى floor
```php
تقريب_لأسفل( $الرقم );
النتيجة: رقم
```

- **تقريب_إلى_فواصل()** - تقريب إلى عدد محدد من الفواصل round
```php
تقريب_إلى_فواصل( $الرقم , $الفواصل = 0 );
النتيجة: رقم
```

- **هل_الرقم_محدود()** - إذا كان الرقم محدود is_finite
```php
هل_الرقم_محدود( $الرقم );
النتيجة: true أو false
```

- **هل_الرقم_غير_محدود()** - إذا كان الرقم غير محدود is_infinite
```php
هل_الرقم_غير_محدود( $الرقم );
النتيجة: true أو false
```

- **هل_المتغير_غير_رقمي()** - إذا كان المتغير غير رقمي is_nan
```php
هل_المتغير_غير_رقمي( $المتغير );
النتيجة: true أو false
```

- **جلب_الأعلى()** - جلب الرقم الأقل من ضمن مجموعة أرقام max
```php
جلب_الأعلى( [ الرقم1 , الرقم2 [, الرقم3] -. ] );
جلب_الأعلى( الرقم1 , الرقم2 [, الرقم3] -. );
النتيجة: رقم
```

- **جلب_الأقل()** - جلب الرقم الأقل من ضمن مجموعة أرقام min
```php
جلب_الأعلى( [ الرقم1 , الرقم2 [, الرقم3] -. ] );
جلب_الأعلى( الرقم1 , الرقم2 [, الرقم3] -. )
النتيجة: رقم
```

- **توليد_رقم_بين()** - توليد رقم بين رقمين mt_rand
```php
توليد_رقم_بين( الرقم_الأقل , الرقم_الأعلى );
النتيجة: رقم
```

### عمليات الجلسات و الكوكيز

$_COOKIE , $_SESSION

- **هل_الكوكيز_مضاف()** - إذا كان الكوكيز المطلوب قد تم إدخاله
```php
هل_الكوكيز_مضاف( $الاسم );
النتيجة: true أو false
```

- **جلب_الكوكيز()** - جلب قيمة الكوكيز
```php
جلب_الكوكيز( $الاسم );
النتيجة: نص
```

- **تعديل_الكوكيز()** - تعديل قيمة الكوكيز
```php
تعديل_الكوكيز( $الاسم , $القيمة , $المدة = 86400 
```

- **حذف_الكوكيز()** - حذف الكوكيز واحدة أو الكل
```php
حذف_الكوكيز( [$الاسم] );
حذف واحدة أو الكل
```

- **تفعيل_الجلسات()** - قبل استخدام الجلسات يجب تشغيل العملية هذه session_start();
```php
تفعيل_الجلسات();
```

- **هل_الجلسة_مضافة()** - إذا كانت الجلسة تم إضافتها
```php
هل_الجلسة_مضافة( $الاسم );
النتيجة: true أو false
```

- **جلب_الجلسة()** - جلب قيمة الجلسة
```php
جلب_الجلسة( $الاسم );
النتيجة: نص
```

- **تعديل_الجلسة()** - تعديل قيمة الجلسة
```php
تعديل_الجلسة( $الاسم , $القيمة );
```

- **حذف_الجلسات()** - حذف الجلسات واحدة أو الكل
```php
حذف_الجلسات( [$الاسم] );
حذف واحدة أو الكل
```

### عمليات بوست و جيت و فايل

$_POST , $_GET , $_FILES

- **هل_متغير_بوست_معرف()** - إذا كان هناك بيانات بوست تم استلامها واحدة أو الكل
```php
هل_متغير_بوست_معرف( [$الاسم] );
النتيجة: true أو false
```

- **جلب_بوست()** - جلب قيمة متغير بوست واحد أو الكل
```php
جلب_بوست( [$الاسم] );
النتيجة: نص أو مصفوفة
```

- **هل_متغير_جيت_معرف()** - إذا كان هناك بيانات جيت تم استلامها واحدة أو الكل
```php
هل_متغير_جيت_معرف( [$الاسم] );
النتيجة: true أو false
```

- **جلب_جيت()** - جلب قيمة متغير جيت واحد أو الكل
```php
جلب_جيت( [$الاسم] );
النتيجة: نص أو مصفوفة
```

- **هل_متغير_المرفق_معرف()** - إذا كان هناك ملفات تم استلامها واحدة أو الكل
```php
هل_متغير_المرفق_معرف( [$الاسم] );
النتيجة: true أو false
```

- **جلب_المرفق()** - جلب بيانات المرفقات واحد أو الكل
```php
جلب_المرفق( [$الاسم] );
النتيجة: مصفوفة
```

- **جلب_اسم_المرفق()** - جلب الاسم الحقيقي للمرفق
```php
جلب_اسم_المرفق( $الاسم );
النتيجة: نص
```

- **جلب_الاسم_المؤقت_للمرفق()** - جلب الاسم المؤقت للمرفق
```php
جلب_الاسم_المؤقت_للمرفق( $الاسم );
النتيجة: نص
```

- **جلب_حجم_المرفق()** - جلب حجم المرفق
```php
جلب_حجم_المرفق( $الاسم );
النتيجة: رقم
```

- **جلب_نوع_المرفق()** - جلب نوع المرفق
```php
جلب_نوع_المرفق( $الاسم );
النتيجة: نص
```

### عمليات الملفات

- **جلب_محتويات_ملف()** - جلب محتويات ملف من السيرفر أو موقع آخر file_get_contents
```php
جلب_محتويات_ملف( $الرابط );
النتيجة: نص
```

- **حذف_ملف()** - حذف ملف من السيرفر unlink
```php
حذف_ملف( $الاسم );
النتيجة: true أو false
```

- **إعادة_تسمية_ملف()** - إعادة تسمية ملف على السيرفر rename
```php
إعادة_تسمية_ملف( $الملف , $الاسم_الجديد );
النتيجة: true أو false
```

- **معلومات_الرابط()** - معلومات الرابط pathinfo
```php
معلومات_الرابط( $الرابط );
النتيجة: نص
```

- **إنشاء_مجلد()** - إنشاء مجلد على السيرفر mkdir
```php
إنشاء_مجلد( $الاسم );
النتيجة: true أو false
```

- **هل_الرابط_مجلد()** - هل الرابط مجلد is_dir
```php
هل_الرابط_مجلد( $الرابط );
النتيجة: true أو false
```

- **نسخ_ملف()** - نسخ ملف copy
```php
نسخ_ملف( $الملف_الأساس , $الملف_الوجهة );
النتيجة: true أو false
```

- **جلب_رابط_المجلد()** - جلب رايط المجلد dirname
```php
جلب_رابط_المجلد( $الرابط );
النتيجة: نص
```

- **جلب_اسم_الملف()** - جلب اسم الملف basename
```php
جلب_اسم_الملف( $الرابط [, $اللاحقة] );
النتيجة: نص
```

- **هل_الملف_موجود()** - إذا كان الملف موجود file_exists
```php
هل_الملف_موجود( $الرابط );
النتيجة: true أو false
```

- **قراءة_ملف()** - قراءة محتويات ملف من السيرفر
```php
قراءة_ملف( $الرابط );
النتيجة: نص
```

- **كتابة_ملف()** - كتابة نص إلى ملف على السيرفر
```php
كتابة_ملف( $الرابط , $البيانات );
```

- **رفع_ملف()** - رفع ملف إلى السيرفر move_uploaded_file
```php
رفع_ملف( $الاسم , $الوجهة );
$الاسم: الاسم المؤقت للملف جلب_الاسم_المؤقت_للمرفق()
$الوجهة: رابط الملف الجديد مع اللاحقة
النتيجة: true أو false
```

### عمليات قواعد البيانات

Mysql

- **إنشاء_اتصال()** - إنشاء اتصال mysql جديد
```php
إنشاء_اتصال( $المضيف , $اسم_المستخدم , $كلمة_المرور , $قاعدة_البيانات );
النتيجة: الاتصال
```

- **آخر_مدخل()** - جلب معرف آخر صف تم إدخاله في قاعدة البيانات insert_id
```php
آخر_مدخل( $الاتصال );
النتيجة: رقم
```

- **طلب_قاعدة_بيانات()** - إدخال ، تعديل ، حذف أو جلب بيانات من قاعدة البيانات
```php
طلب_قاعدة_بيانات( $الاتصال , $الطلب , $تحديث_أو_حذف_أو_إدخال = خاطئ );
النتيجة: نص , true أو false
```

يمكن كتابة الطلب باللغة العربية داخل أو خارج القالب

**مثال - إنشاء الاتصال**
```php
$الاتصال = إنشاء_اتصال( "localhost" , "root" , "" , "testdb" );
النتيجة: الاتصال
```

**مثال - حذف**
```php
$الحذف = طلب_قاعدة_بيانات( $الاتصال , "ع.حذف ع.من table ع.عندما_يكون id=1" , صحيح );
النتيجة: true أو false
```

**مثال - تعديل**
```php
$التعديل = طلب_قاعدة_بيانات( $الاتصال , "ع.تحديث table ع.إعداد name='عبدالستار'،age='29' ع.عندما_يكون id=1" , صحيح );
النتيجة: true أو false
```

**مثال - إدخال**
```php
$الإدخال = طلب_قاعدة_بيانات( $الاتصال , "ع.إدخال table (name،age،mail) ع.القيم('عبدالستار'،29،'AboAlimk@gmail.com')" , صحيح );
النتيجة: true أو false
```

**مثال - جلب**
```php
$البيانات = طلب_قاعدة_بيانات( $الاتصال , "ع.جلب name،age،mail ع.من table ع.عندما_يكون id=1 ع.أو id=2 ع.الترتيب id ع.تصاعدي ع.حد 1" );
النتيجة: مصفوفة
array( "عدد_الصفوف" => 5 , "الصفوف" => array())
```

**مايمكن كتابته بالعربي ضمن طلب Mysql**
```php
،   -   ,
ع.جلب   -   select
ع.من   -   from
ع.عندما_يكون   -   where
ع.حد   -   limit
ع.العدد   -   count
ع.حذف   -   delete
ع.تحديث   -   update
ع.الترتيب   -   order by
ع.تصاعدي   -   asc
ع.تنازلي   -   desc
ع.أعلى   -   max
ع.أقل   -   min
ع.إدخال   -   insert into
ع.القيم   -   values
ع.إعداد   -   set
ع.و   -   and
ع.أو   -   or
```

ويمكن استخدام كافة متغيرات Mysql الإفتراضية إذا احتجت لذلك

### مثال لاستخدام المكتبة عدة مرات في نفس الصفحة

المثال يفترض أن الموقع يقوم بتحويل جميع الصفحات إلى index.php

ملف .htacces

```
<IfModule mod_rewrite.c>
RewriteEngine On
RewriteRule ^index\.php$ - [L]
RewriteCond %{REQUEST_FILENAME} !-d
RewriteCond %{REQUEST_FILENAME} !-f
RewriteRule . /index.php [L]
</IfModule>
```

ملف index.php

```php
<?php
require_once 'Arabic-PHP-Engine.php';

$ع = new ع;

$الفروع = جلب_مصفوفة_الفروع();

$الطلب = $الفروع[ 0 ];

if( $الطلب == "home" ){
	
	$ع->تضمين("home.php");
	
} else if( $الطلب == "about" ) {
	
	$ع->تضمين("about.php");
	
} else if( $الطلب == "contact-us" ) {
	
	$ع->تضمين("contact-us.php");
	
} else {
	
	$ع->تضمين("error-404.php");
	
}
```






**المكتبة مفتوحة المصدر ويمكن للجميع تعديلها أو تطويرها**

</div>