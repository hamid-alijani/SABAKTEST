SABAK 

شرح پروژه: 

در این پروژه دو صفحه وجود دارد.
صفحه اول شامل هدر - سکشن افزودن کاربر - سکشن لیست کاربران و 
صفحه دوم شامل هدر - سکشن ویرایش کاربر

صفحه اول شامل یک فرم می باشد برای افزودن کاربر که فیلد های این فرم:
نام: کاربر می تواند هر ورودی را وارد کند.
نام خانوادگی: کاربر می تواند هر ورودی را وارد کند.
نام پدر: کاربر می تواند هر ورودی را وارد کند
شماره همراه: حتما باید عدد یازده رقمی باشد
تحصیلات: به صورت select option (انتخابی) باشد که شامل :
grade selcet option = [
 { value : 1 , label: "دیپلم"},
 { value: 2, label: "لیسانس" }
]
است.
دانشگاه: در صورت انتخاب تحصیلات لیسانس این فیلد باید نمایش داده شود. و کاربر می تواند هر ورودی را وارد کند.

پس از ثبت یک کاربر جدید و موفقیت آمیز بودن آن، رکورد جدید باید به لیست پایین صفحه اضافه شود.
در صورت کلیک روی دکمه ویرایش موجود در لیست، کاربر باید به صفحه جدید:
/info/:id
فرستاده شود و در آن صفحه ابتدا اطلاعات کاربر مورد نظر (id) دریافت شود و فیلد های موجود پر شود و سپس امکان ویرایش و ثبت اطلاعات وجود داشته باشد.
پس از ویرایش اطلاعات کاربر به صفحه اصلی برگردانده شود.



- تمامی فرم ها باید با استفاده از formik مدیریت شوند
- برای ولیدیشن از کتابخانه yup استفاده شود 
- برای ارسال درخواست های http و دریافت داده از کتابخانه های Axios و react query استفاده شود
- در قسمت افزودن و ویرایش کاربر، تمامی فیلد ها الزامی هستند
- فیلد دانشگاه در صورتی الزامی است  که گزینه انتخاب شده برای تحصیلات لیسانس باشد
- شماره تلفن همراه باید عدد و 11 رقم باشد ( از yup برای ولیدیشن استفاده شود)
- پیام خطا برای اینپوت هایی که valid نباشند باید زیر آن اینپوت نمایش داده شود
- نیاز به pagination برای لیست وجود ندارد
- کل پروژه باید با زبان typescript توسعه داده شود


- توجه : در این پروژه اولویت روی درست کار کردن کامپوننت ها می باشد
- در صورت زیبایی ظاهری پیاده سازی ui امتیاز مثبت تعلق می گیرد
- برای استایل دهی می توانید از css module استفاده کنید
- در صورت استفاده از scss امتیاز مثبت تعلق می گیرد.
- در صورت استفاده از کتابخانه reactstrap برای پیاده سازی گرید امتیاز مثبت تعلق میگیرد


wire frame : https://wireframepro.mockflow.com/view/MRRvJaLp8h


CREATE USER INFO - ( POST REQUEST )
https://6249e521fd7e30c51c085463.mockapi.io/api/info

{
  "name": "",
  "lastname": "",
  "fatherName": "",
  "phoneNumer": "",
  "grade": 1, // [1 , 2 ]
  "university": ""
}

- تنها در صورتی فیلد دانشگاه نمایش داده شود که  تحصیلات انتخابی لیسانس باشد


GET LIST - ( GET REQUEST)
https://6249e521fd7e30c51c085463.mockapi.io/api/info

GET BY ID - ( GET REQUEST ) 
https://6249e521fd7e30c51c085463.mockapi.io/api/info/:id

UPDATE BY ID - ( PUT REQUEST )
https://6249e521fd7e30c51c085463.mockapi.io/api/info/:id


پس از اتمام پروژه، فایل های پروژه به همراه نام و نام خانوادگی به آدرس hamidalijaniw@gmail.com ایمیل شود.