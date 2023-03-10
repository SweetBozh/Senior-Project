# User Function `(User ทำอะไรได้บ้าง)`

- Register
- Login
- Search Place
- Recommended User
- Recommended Place
- My Plans
- Plan Today
- View Plan
- Create Plan
- Search Existing Plan
- Delete Plan
- Custom Plan
- Review Place
- View Profile

# Function Details

## Register

- username
- password
- confirm password
- email
- full name

## Login

- username
- password

# Home Page

## Search Place

- Recommended Sort
- View Place
  * Like
  * Already Visited
  * Description
  * Rating
  * Review Place`(คนยังไม่ไปก็มารีวิวได้)`
  * Open - Close Time
  * Pinned
  * Added to Trip
  * Tel `(ดึง Google API, copy พาไปหน้าโทร)`
  * Share
  * View Map
- View User

## Recommended Traveler `(ดู Top User เพื่อเข้าไปดู Profile เขา)`

- อาจมีการจัดกลุ่ม User

## Recommended Place `(แนะนำสถานที่เที่ยวที่น่าสนใจจากแอพเราเอง)`

- Rating top 5 in Thailand (Google API)
- Recommended by user (Top Rate, Influencer)
    `{วัดตามยอด Follow, ยอด Review สถานที่}`

## View Profile

* Share Profile
* Follow Profile
* View MyPlans
      > - (Set this plan public/private)
      > - Hide Starting Point (For Privacy of public plan)
      > - Plan Detail
      > - Share
      > - Create from this plan
* View Photos
* Like Plan

### My Plans `ดูแพลนของฉัน`

- แพลนที่ยังไม่เสร็จ `(Max 5, ขึ้นเครื่องหมาย ! ถ้าเลยวันที่ที่ใส่ไว้แล้ว)`
- เริ่มต้นไปตามแพลน `ปุ่ม Start Trip`
- แพลนที่เสร็จสิ้นแล้ว `(ถ้า Start Trip แล้ว พอเลยวันที่นั้นแล้ว จะ Pop-up เพื่อบอกว่า Plan นี้สิ้นสุดยัง)`

## Plan today `Pattaya Plan, Day 1 2 3 4`

- Place List (เลือก Review จากลิสต์สถานที่)
- add place
- remove place
- Move place to day....
- Remove Day
- Add Day
- Destination จังหวัดเปลี่ยนตาม Place สุดท้ายของ Plan ใน Day สุดท้าย

## Create Plan `สร้างแพลนด้วยตนเอง เพิ่มลงใน {ฐานข้อมูลแพลน}`

### Search Existing Plan `เที่ยวตามแพลนคนอื่นที่มีอยู่แล้ว Fork เป็น My Plan แล้วไป Custom ต่อได้`

- (optional) เลือก Source, Destination
- (optional) เลือก `{budget, price level}`
- เลื่อนขยายดูเพิ่มได้เรื่อยๆ (Extended Layout)
- Recommend Plan จะแสดง Source, Destination ของ Plan นั้น
- ถ้าไม่เลือก Source, Destination จะ Recommend Plan ตาม Rating
- ถ้าเลือก Source, Destination จะ Recommend Plan ได้ 2 แบบ `{Related, Rating}`
- สามารถเลือก Feature 'Hide Starting Point' ได้ (Privacy)

### Create My Own `สร้างแพลนของตัวเอง`

- เลือกสถานที่ต้นทางและปลายทาง `กรุงเทพ -> เขาใหญ่ สามารถปรับแต่งขณะ Custom ได้`
  * Add place on the way `กรุงเทพ -> สุพรรณ -> เขาใหญ่`
- เลือกจำนวนวัน
- (optional) เลือก `{
  * budget เงินเริ่มต้น
  * price level ระดับความแพงของสถานที่
     <!-- * vehicle
     > - เครื่องบิน
       1. ให้เลือกสนามบินที่ขึ้น - ลง
       2. กรุงเทพ -> ดอนเมือง -> เชียงใหม่ -> ดอนเมือง -> กรุงเทพ
       3. กรุงเทพ -> 
       ไม่แวะระหว่างทาง เปลี่ยนไปเที่ยวรอบๆ Destination `เช่น จาก กรุงเทพ -> เชียงใหม่ แต่ไฟลท์ว่างแค่เชียงราย (ให้ User เลือกสนามบิน -> Source จะกลายเป็นสนามบิน กับจังหวัดของสนามบินนั้น -> แล้วให้ใส่ Destination ใหม่)`
     > - ขับรถไปเอง/เช่ารถ แวะระหว่างทาง ใช้ Default -->

- เลือก `{Auto Plan ให้แอพจัดแพลนให้เลย random ให้, Self Plan จัดแพลนด้วยตัวเอง}`
  * Auto Plan 
    > - สุ่มให้หมดทุกอย่างครบจบ

  * Self Plan (which can random place)
     > - พิมพ์ชื่อสถานที่ที่จะไป
     > - สามารถเลือกชอยส์ Random 'Place Type' เช่น Random 'ร้านอาหาร' จาก dropdown อันแรกได้ `(โดย Type ดึงจาก Place Type API ของ google)`
     > - เดิมเป็น price level ที่ option ไว้เป็น default ของทุกที่, แต่มีปุ่มให้ edit price level ของแต่ละที่ได้

- ปรับแต่งแพลนเพิ่มเติม
  * ตรวจสอบแพลนของแต่ละวัน
  * Add Place
     > - search สถานที่ `{rating, price level, type place}`
     > - Recommended สถานที่
  * Delete Place
  * Set route `(ปรับแต่งเส้นทาง)`
  * Share to plan together

    * Save (auto saved)
    * Finish (Congrat!)
    ??? Add Hotel

## Delete Plan `ลบแพลนจากรายการแพลน`

- ถามยืนยันการลบ

### Like after travel

- ให้หัวใจน้องมาสคอตของแอพ

- สถานที่หรือจังหวัดน่าไป 1 - 10 จัด plan เอง 1. 2. 3. ก่อนเซิร์ช อยากไปเที่ยวแต่ไม่รู้จะไปไหน

Discuss next meeting
- Hotel
- Budgeting Plan

<!-- 
- Testing หลังเที่ยว
- เก็บข้อมูลจาก user เพื่อเอามาใช้ต่อ
เช่น คนนี้ชอบเที่ยวเขา - ประหยัด
เพื่อเอาข้อมูลมาใช้ต่อ 
:. จะเก็บข้อมูลอะไรบ้าง จากไหน ตอนสมัครมั้ย ชอบเที่ยวแบบไหน สายไหน (ตย.)
ระบบ Recommend: ชอบทะเล งั้นแนะนำสถานที่ที่คนอื่นเคยไป แล้วเป็นทะเล
- ประหยัด, เลือกตอนเข้าแอพ ใส่กับทุกแพลนที่ user จะเลือก
- ทุกครั้งที่สร้างแพลน ให้เลือกประเภท

- สมัครได้ -> แนะนำเวลาทำ Default plan,
เวลาเลือกสถานที่ ขึ้นแบบ Wanderlog 
เก็บสถิติว่าปกติเลือกแบบไหน
- Native, Flutter , kotlin -->
