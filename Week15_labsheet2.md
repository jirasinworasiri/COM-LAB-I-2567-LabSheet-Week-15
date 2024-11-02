# การทดลอง
## การ debug .NET console application โดยใช้ Visual Studio Code

ใบงานนี้จะทำการ debug .NET console application โดยใช้ Visual Studio Code

## การเตรียมการเบื้องต้น
- โปรแกรม HelloWorld ที่สร้างในใบงาน [Week15_labsheet1.md](./Week15_labsheet1.md)

## การ debug application

1. แก้ไขโปรแกรมในเมธอด `static void Main(string[] args)` ของ ไฟล์ `Program.cs`

![alt text](./Pictures/image-15.png)

2. เพิ่มเมธอด `static int Add(int var1, int var2)`

![alt text](./Pictures/image-16.png)

3. ตรวจสอบให้แน่ใจว่าไฟล์ `Program.cs` มีเนื้อหาดังต่อไปนี้

![alt text](./Pictures/image-17.png)

4. คลิกที่แถบด้านซ้ายตัวเลขบรรทัด เพื่อตั้ง break point ที่บรรทัด  `int a = 1;`

![alt text](./Pictures/image-18.png)

5. กด F5 เพื่อ debug โปรแกรม

![alt text](./Pictures/image-19.png)

6. เมื่อแถบสีเหลืองปรากฏบนบรรทัดที่ 7 ให้สังเกตุค่าตัวแปรต่างๆ ในหน้าต่างย่อย VARIABLES 

 ![alt text](./Pictures/image-20.png)

7. กดปุ่ม Step Over (F10) 

![alt text](./Pictures/image-21.png)

8. สังเกตุหน้าต่าง Program.cs และหน้าต่างย่อย VARIABLES แต่ละขั้นของการ Step over ไปทีละบรรทัดจนจบโปรแกรม

**บันทึกผลการทดลอง**
ผลที่ได้จากการทำงานในแต่ละบรรทัด  ถูกต้องตามที่เขียนเขียนโปรแกรมไว้หรือไม่

**หมายเหตุ**
ในการ debug เราสามารถใช้ command pallette ในการสั่งการได้ 

สามารถเรียกโดยใช้ Ctrl+Shift+P  แล้วพิมพ์ debug ลงในช่องค้นหาคำสั่ง ดังตัวอย่าง

![alt text](/Pictures/image-22.png)

9. ตรวจสอบให้แน่ใจว่าตั้ง break point ไว้ที่บรรทัดที่ 7 แล้ว รันคำสั่ง Debug:Start Without Debugging     

![alt text](./Pictures/image-23.png)

**บันทึกผลการทดลอง**
- การรันคำสั่ง Start Without Debugging ให้ผลเหมือนหรือต่างจากการ debug
- ![image](https://github.com/user-attachments/assets/f1cb7dfd-35e4-4e34-a8f7-c157d66912b7)

- การตั้ง break point มีผลอย่างไรกับการรันในโหมด Start Without Debugging หรือไม่
- ![image](https://github.com/user-attachments/assets/37639f3f-016a-49de-915d-7d5a04f7f6db)



