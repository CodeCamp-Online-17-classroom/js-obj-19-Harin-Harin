# js-lab-65
### Lab65 Object: Guess Result4
บรรทัดที่มี * ให้ผลลัพธ์เป็นอะไร เพราะอะไร   
ผลลัพท์ เป็น Joe เพราะ ref:this = window (ไม่ได้อยู่ใน object แต่อยู่ในหน้าจอหลัก)     
        user.ref.name = var name คือ Joe     
        ส่วน user.name คือ John      
หริณ มาเบ้า

```JavaScript
var name = 'Joe';
function makeUser() {
  return {
    name: 'John',
    ref: this
  };
}
let user = makeUser();
console.log(user.ref.name); // *
```
