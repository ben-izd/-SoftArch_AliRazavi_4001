# -SoftArch_AliRazavi_4001
Software Architecture Assignments for 1400-1401-1 semester by Ali Razavi 

<div style="direction: rtl;">

## نیمه اول

### تعریف معماری نرم‌افزار و نحوه ارزیابی آن

مجموعه‌ای از ساختارهای مختلف که امکان گفتگو درباره ابعاد گوناگون یک سیستم را فراهم می‌کند. ساختارهای متنوعی برای افراد مختلف برنامه‌ریزی شده است. مثلاً برای تیم توسعه ساختاری که نشان‌دهنده اجزای سیستم و نحوه ارتباط آنها با هم یا برای کاربران یا سرمایه‌گذاران، ساختار کلی سیستم و برنامه‌ریزی زمانی و تخمین سرمایه مورد نیاز در نظر گرفته شده است. هر پروژه متناسب با نیاز و محدودیت‌های خاص خود، به تعدادی از این نوع ساختارها نیاز دارد. مناسب بودن یا نبودن یک معماری با در نظر گرفتن بستر پروژه ارزیابی می‌شود و هر پروژه حتی بدون مستندات لازم نیز، نوعی معماری را داراست.

معماری سطحی انتزاعی از پروژه است که از ساختارهایی تشکیل شده که این ساختارها از عناصر و روابط بین آنها شکل می‌گیرد. معماری با حذف عناصر غیرضروری (مربوط به پیاده‌سازی داخلی) و در نظر گرفتن رفتار ضروری (مرتبط با صفات کیفی) امکان فهم پروژه بصورت کلی و ارزیابی صفات کیفی مد نظر را می‌دهد.
ساختارهای معماری را می‌توان بصورت کلی به سه ساختار تقسیم کرد:

- مولفه و ارتباط دهنده: ساختار سیستم را بشکل مجموعه‌ای از عناصری که در زمان اجرا، رفتاری انجام‌می‌دهند (مولفه) و تعامل آنها (ارتباط دهنده) توصیف می‌کند. مولفه‌ها واحدهای کلی پردازشی مثل سرور، کلاینت یا موارد دیگر و ارتباط دهنده‌ها، وسیله ارتباطی میان مولفه‌ها مثل لوله‌ها و ... هستند.

- واحد (ماژول): ساختار سیستم را به بخش‌های اجرایی تقسیم می‌کند. این واحدها، هر کدام مسئولیتی پردازشی دارند که بدون تاکید برنحوه اجرا، پایه تخصیص وظایف به تیم‌های برنامه‌نویسی هستند.

- تخصیص: ساختارهای نرم‌افزاری را به ساختار غیرنرم‌افزاری مثل سخت‌افزار، تیم‌های توسعه و ... مرتبط می‌کند.

برای ارزیابی یک معماری می‌توان از مراحل زیر استفاده کرد:

0. تشکیل تیم ارزیابی می‌تواند شخص معمار یا همکارانش یا تیم مجزا از بخش یا شرکت باشد
1. اطمینان از درک کامل معماری توسط تک تک افراد تیم ارزیابی
2. تعیین سناریوهای صفات کیفی اولویت‌دار برای ارزیابی معماری
3. برای هر سناریو، معمار یا مستندات باید بطور کامل نحوه دستیابی به صفات کیفی مد نظر را توجیه کرده و تیم ارزیابی در صورت مخالفت، طرح‌های جایگزین برای قسمت مد نظر ارائه کند.
4. تیم ارزیابی، مشکلات مطرح شده در قسمت قبل را ضبط و پیگیری نماید.

نکته قابل توجه، انعطاف‌پذیری در تحلیل است. بعنوان مثال تصمیماتی که برای دستیابی به یک صفت کیفی اولویت‌دار گرفته شده ارزش بالاتری از سایر تصمیمات دارد. همچنین، دنبال جایگزین ایده‌آل نبایشد. بعد از رسیدن به جایگزینی مناسب، به سراغ مراحل بعدی روید.


## نیمه دوم

### تشریح کامل مدل یک صفت کیفی

در اینجا از Usability بعنوان مثال برای تشریح مدل صفت کیفی استفاده می‌شود.
هر صفت دامنه از ویژگی‌ها را برای سیستم در نظر می‌گیرد مثلاً برای صفت مدنظر:

- یادگیری ویژگی‌های سیستم: مقدار زمان و تلاشی که یک فرد غریبه برای کار با سیستم هزینه کند.
- استفاده بهینه از سیستم: ارائه قابلیت‌هایی که منجر به کارآمدی شود.
- کمینه‌کردن خطا کاربری: جلوگیری از ایجاد خطا در سیستم توسط کاربر مثل محدود کردن قابلیت‌ها و ...
- توجه با نیاز شخصی هر کاربر: ارائه ویژگی‌هایی منحصر به کاربر
- افزایش احساس اطمینان: دادن بازخورد به کاربر تا از فعالیت سیستم مطمئن باشد.

هر صفت می‌تواند به سایر صفات وجه مشترکی داشته باشد که اصلاح در هر کدام، در هر دو تأثیر گذار است. برای مثال صفت Usability، با صفت modifiability مشترک است مثلاً برای تست رابط‌های گوناگون، به سیستم خواهید رسید پذیرای تغییرات باشد.

هر صفت از یک جدول سناریو عمومی و چند سناریو واقعی (Concrete) تشکیل شده است که برای صفت Usability موارد زیر در نظر گرفته شده:

</div>

| جزء سناریو | مقدار احتمالی |
| :------------- | -------------: |
| Source | منبع یا سر منشاء محرک – کاربر حرفه‌ای یا واکنش کاربر به یک رویداد |
| Stimulus | محرک یا درخواست کاربر – یادگیری سیستم، بکارگیری بهینه سیستم، کاهش خطای کاربر و موارد دیگر |
| Environment | محیط یا فضایی که درخواست ارسال می‌شود – درخواست‌ها در زمان اجرا یا تنظیم ارسال می‌شوند. |
| Artifacts | محرک به کدام قسمت اثر می‌گذارد – رابط کاربری |
| Response | پاسخ یا واکنشی که سیستم می‌دهد – ارائه ویژگی مدنظر کاربر – پیش‌بینی نیاز |
| Response Measure | نحوه اندازه‌گیری پاسخ – اندازه تعداد خطاها یا زمان یادگیری یا رضایت کاربر یا موارد دیگر |

<div style="direction: rtl;">

مثالی برای سناریو معین:

کاربر برنامه‌ای جدید نصب کرده و در 10 دقیقه، با سعی و خطا توانست به خوبی از سیستم استفاده کند.

بطور معمول برای اکثر صفات معروف، تاکتیک‌ها و الگوهایی شناسایی و طراحی شده که استفاده از آنها، رسیدن به سطح بالایی از صفت مورد نظر را آسان می‌کند. برای صفت Usability، توانایی کنسل، Undo، توقف و ادامه یا کمک به کاربر براساس تجربه قبلی کار با سیستم و موارد دیگر را می‌توان نام برد. برای تاکتیک‌های ذکر شده، می‌توان لیستی تهیه کرد تا پشتیبانی، دلایل موافقت یا رد، ریسک‌های احتمالی و تصمیمات ضروری برای پیاده‌سازی آنها را نیز مستندسازی کرد.

### طراحی و ساخت سناریو عمومی و معین یک صفت کیفی تخیلی

با تکیه بر واژه تخیلی بدون در نظر گرفتن عواقب مالی و قانونی، صفت Crackability یا قابلیت شکسته شدن (لایسنس) انتخاب شده است (واژه در سطح اینترنت استفاده شده ولی با تکیه بر دانش فردی پاسخ نوشته شده است).

زندگی در کشور جهان سومی با عقایدی که منجر به نپذیرفتن قانون کپی‌رایت جهانی شده، در کنار شرایط اقتصادی و نسبت پائین درآمد متوسط برای خرید کالاهای جهانی، به ناچار با نرم‌افزارهای قفل شکسته آشنا می‌شویم. از یک ویندوز و آفیس ساده تا نرم‌افزارهای تخصصی رشته‌های گوناگون، غالباً یک جستجو فاصله است. بدون در نظر گرفتن عواقب و یا مزایای آن (هم برای افراد استفاده کننده و هم صاحب محصول)، قصد داریم به این واژه، بعنوان یک صفت کیفی نگاه کنیم.

برخلاف اکثر صفات کیفی که رسیدن به سطح بالایی از آنها نیاز به تلاش و صرف هزینه است، در این صفت با کم کردن هزینه می‌تواند به سطح قابل قبولی رسید. البته منظور حفظ تعادلی است که مشتریانی که توانایی مالی دارند را به سمت استفاده از نسخه قفل شکسته سوق ندهد و از آن طرف امکان شکستن آن به افرادی که شرایط مورد نیاز را ندارند، فراهم کند.

</div>
  
| جزء سناریو | مقدار احتمالی |
| :------------- | ------------: |
| Source | هکرها |
| Stimulus | نفوذ به محصول - تولید سریال |
| Environment | بدون دسترسی به اینترنت - با دسترسی به اینترنت - اشکال زدایی |
| Artifacts | احراز هویت - تائید لایسنس - تولید سریال |
| Response | قبول هویت - قبول لایسنس |
| Response Measure | در سیستم: ارسال مشخصات کاربر <br> خارج از سیستم: فاصله عرضه و شکسته شدن قفل در انجمن‌های تخصصی - بررسی محتوا با تمرکز این محصول در زبان‌ها و مناطق مختلف دنیا |

<div style="direction: rtl;">

سناریو معین:

هکرها یک ماه پس از عرضه نرم‌افزار، توانستند با مهندسی معکوس در محیط اشکال‌زدایی، الگوی تولید سریال را بدست آورده و آن را در انجمن‌های تخصصی قرار دهند.

سناریو معین در دنیای واقعی:

گروه CODEX قفل UWP مایکروسافت در بازی Zoo Tycoon Ultimate Animal Collection را پس از یکسال کرک کرد.

هکرها قفل Denuvo بازی TEKKEN 7 را چهار روز بعد از انتشار، شکستند.




</div>


