# <div dir="rtl" align="right">+R یادداشتی در مورد ریسک ها</div>  

## <div dir="rtl" align="right">این بخش درباره ریسک‌هایی است که از ضعف ها نشات میگیرند.</div>

<p dir="rtl" align="right">روش رتبه بندی ریسک Top 10 بر پایه <a href="https://wiki.owasp.org/index.php/OWASP_Risk_Rating_Methodology">روش رتبه بندی ریسک OWASP</a> است. برای هر دسته TOP 10 ما ریسکی را که هر ضعف به یک برنامه کاربردی تحت وب معرفی می‌کند را با نگاه به فاکتورهای احتمال و تأثیر برای هر ضعف متداول، تخمین می‌زنیم. سپس TOP 10 را بر اساس آن ضعف‌ها که به صورت نوعی مهم‌ترین ریسک برای یک برنامه را مشخص می‌کند، مرتب می‌کنیم. این فاکتورها با هر بار انتشار جدید TOP 10 به‌روز می‌شوند چون همه چیز تغییر می‌کند و تکامل می‌یابد.</p>

<p dir="rtl" align="right"><a href="https://wiki.owasp.org/index.php/OWASP_Risk_Rating_Methodology">روش رتبه بندی ریسک OWASP</a> فاکتورهای متعددی برای کمک به محاسبه ریسک یک برنامه شناخته شده ارائه می‌کند. اگرچه TOP 10 بیشتر درباره کلیات صحبت می‌کند تا آسیب‌پذیر‌ی‌های خاصی در برنامه‌های واقعی و API ها. در نتیجه ما هیچ وقت نمی‌توانیم به اندازه صاحب یا مدیر یک برنامه دقیق باشیم وقتی که برای برنامه‌(ها)ی آنها ریسک را محاسبه می‌کنیم. شما بهترین فرد برای قضاوت درباره اهمیت برنامه‌ها و داده‌هایتان هستید، تهدید‌های شما چه هستند و چگونه سیستم شما ساخته شده است و کار می‌کند.</p>

<p dir="rtl" align="right">روش ما شامل سه فاکتور احتمالی برای هر آسیب‌پذیری است (شیوع، قابلیت تشخیص و سادگی بهره‌جویی) و یک فاکتور تأثیر (تأثیر فنی). مقیاس ریسک که برای هر فاکتور در بازه کم-1 تا زیاد-3 قرار دارد همراه با واژه‌شناسی برای هر فاکتور تعیین شده. شیوع یک آسیب‌پذیری فاکتوری است که معمولاً لازم نیست محاسبه شود. برای داده شیوع ما آماری از شرکت‌های مختلف تهیه کرده‌ایم (که در بخش تقدیر و تشکر در صفحه 25 آورده شده است) و ما داده‌های آنها را باهم تجمیع کردیم تا با لیست احتمال TOP 10 منطبق شود. این داده‌ها بعدا با فاکتور‌های احتمالی دیگری (قابلیت تشخیص و سادگی بهره‌جویی ) ترکیب شد تا رتبه احتمالی هر آسیب‌پذیری محاسبه شود. رتبه بندی احتمال بعدا با ضرب در تخمین میانگین تأثیرفنی برای هر آیتم محاسبه می‌شود تا به طور کلی با رتبه‌بندی ریسک برای هر آیتم در TOP 10 (نتیجه بالاتر به معنی ریسک بالاتر است) همراه باشد. قابلیت تشخیص، سادگی بهره‌جویی و تأثیر از آنالیز گزارش‌های CVE که با هر دسته TOP 10 ترکیب شده است محاسبه شده است.</p>

<p dir="rtl" align="right"><strong>توجه : </strong>این دیدگاه درباره احتمال عامل تهدید به یک حساب کاربری صحبت نمی‌کند. و همچنین هیچکدام از جزئیات دقیق در ارتباط با یک برنامه خاص را به حساب نمی‌آورد. هرکدام از این فاکتورهای میتوانند به صورت ویژه احتمال کلی اینکه یک مهاجم یک آسیب پذیری خاص را محاسبه کرده و از آن سو استفاده کند. این امتیازدهی تأثیر واقعی روی کسب و کار شما را به حساب نمی‌آورد. سازمان شما باید تصمیم بگیرد که چه مقدار خطر امنیتی از برنامه ها و API ها را میتواند بپذرید، با توجه به فرهنگ شما، صنعت و محیط. هدف OWASP TOP 10 این نیست که آنالیز این خطرها را برای شما انجام دهد</p>

<p dir="rtl" align="right">در ادامه توضیح محاسباتی ما برای ریسک در مورد <strong> A6:2017 -  پیکربندی اشتباه امنیتی </strong>. را خواهیم داشت.</p>

![Risk Calculation for A6:2017-Security Misconfiguration](images/0xc0-risk-explanation.png)

