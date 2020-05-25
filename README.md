# BaacLotto-Notify

ระบบแจ้งเตือนผลสลาก ธกส. ผ่าน Line Notify  
โดยจะส่งแจ้งเตือนทุกวันที่ 16

### วิธีใช้งาน

ใส่ Line Token (กดรับ -> [LINE Notify](https://notify-bot.line.me/en/))
```go 
var lineToken = "YOURTOKEN"
```
ใส่ค่าให้ครบ [lottoGroup](#lottogroup), startNo, stopNo
```go
lottoNumber = append(lottoNumber, getLottoResult("lottoGroup", "startNo", "stopNo"))
```
ถ้ามีสลากหลายใบสามารถเพิ่มได้แบบนี้
```go
lottoNumber = append(lottoNumber, getLottoResult("lottoGroup", "startNo", "stopNo"), getLottoResult("lottoGroup", "startNo", "stopNo"))
```

<h3 id="lottogroup">เลข lottoGroup</h3>

- 36 = สลากทวีสิน เกษตรมั่นคง 3 (RA-RT)
- 35 = สลากออมทรัพย์เกษตรยั่งยืน
- 34 = สลากธ.ก.ส.ชุดเกษตรมั่งคั่ง4(ป0-ศ9)
- 33 = สลาก ธ.ก.ส.ชุดเกษตรมั่งคั่ง 3(ด0-บ9)
- 32 = สลากทวีสิน เกษตรมั่นคง 2 (PH-PQ)
- 31 = สลากธ.ก.ส.ชุดเกษตรมั่งคั่ง2(ช0-ณ9)
- 30 = สลากธ.ก.ส.ชุดเกษตรมั่งคั่ง(ก0-ฉ9)
- 29 = สลากทวีสิน ชุดเกษตรมั่นคง(PA-PG)
- 28 = สลาก ธ.ก.ส.ชุดที่ 4(P0-U9)
- 27 = สลากธ.ก.ส. ชุด 3 (I0-N9)
- 26 = ชุดกล้วยไม้นานาชาติ (NM-NW)
- 25 = สลาก ธ.ก.ส. ชุด 2 (C0-H9)
- 24 = สลากทวีสิน 2558 (NG-NL)
- 23 = สลาก ธ.ก.ส. ชุด 1 (01-60)
- 22 = สลากทวีสิน ชุด 2557 (NA-NF)
- 21 = ขวัญแผ่นดิน (M0-MU)
- 20 = บัตรเพิ่มทรัพย์ ชุดที่ 9 (B0-B9)
- 19 = บัตรเพิ่มทรัพย์ ชุดที่ 8 (A0-A9)
- 18 = ข้าวทิพย์ (MH- MN)
- 17 = กล้วยไม้พระนาม (MA-MG)
- 16 = บัตรเพิ่มทรัพย์ ชุดที่ 7 (BK-BT)
- 15 = บัตรเพิ่มทรัพย์ ชุดที่ 6 (BA-BJ)
- 14 = ขวัญข้าว 2 (LN-LT)
- 13 = ขวัญข้าว (LG-LM)