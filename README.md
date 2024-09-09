## Суулгах:
https://pypi.org/project/mongol-register-parser/

эсвэл

```
pip install mongol-register-parser
```

## Ашиглах заавар:
```
from mongol_register_parser import mongol_register_parser

fileName='your_file_name.csv'
register_number_column = "register_number_column_name"

newPandasDataFrame = mongol_register_parser.mongol_register_parser(fileName, register_number_column)
```
## Үр дүн:
newPandasDataFrame дотор age, birthYear,  birthMonth,  birthDay гэсэн баганууд үүснэ.

## Тайлбар:
-Уг parser нь 1930-с 1940 онд хүртэлх төрсөн хүмүүсийг Регистрийн дугаарыг бододгүй.
-Хэрэв буруу Регистрийн дугаар орж ирвэл 1700 оны 01 сарын 01 гэж хадгалдаг тул анхаарна уу.

Монгол регистрийн дугаарын эхний 2 орон буюу үсэг нь регистрийн дугаар авч байгаа иргэний байнга 
оршин суудаг аймаг /дүүрэг/, сум /хороо/-ны код, дараагийн 6 орон нь төрсөн он, сар, өдөр 9 дэх орон нь хүйс, 
сүүлийн нэг орон нь хяналтын код байна.

Регистрийн эхний 2 тоон орон нь тухайн иргэний төрсөн оны сүүлийн 2 тоог тэмдэглэдэг. 
Түүний дараагийн 2 орон төрсөн сарыг илэрхийлэх бөгөөд 2000 он болон түүнээс хойш төрсөн хүмүүсийн
хувьд төрсөн сар дээр нь 20-ийг нэмж тэмдэглэдэг. Харин дараагийн 2 орон төрсөн өдрийг илэрхийлнэ.

Регистрийн дугаарын сүүлээсээ 2 дахь тоо нь хүйсийг заах бөгөөд хэрвээ тус тоо сондгой бол хүйс нь эрэгтэй,
үгүй бол эмэгтэй гэж үзнэ. Харин хамгийн сүүлийн орон бол, тус регистрийн дугаарыг үнэн оруулсан эсэхийг шалгахад
ашиглагддаг тоо болно. Хэрхэн уг тоог ашиглан шалгаж болох талаар нээлттэй эх сурвалжуудад баттай мэдээлэл байхгүй ч,
энэхүү нийтлэлийн коммент хэсэгт уг тоо регистрийн дугаарт орж байгаа үсэг болон тоонуудын нийлбэрийг тодорхой нэг
тоонд хуваасны үлдэгдэлтэй тэнцэх ёстой гэх мэдээлэл байна.