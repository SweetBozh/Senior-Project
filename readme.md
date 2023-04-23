## Page List

- [Login Page]()
  * Login (username, password / Google / Facebook / Email)
  * `Register Page`
  * `Forget Password Page`

- [Register]()
  * Username
  * Password
  * Confirm password
  * Email
  * Firstname
  * Lastname
  * Birthday 
  * `Preference Page ( register )`

- [Forget Password]()
  * Email

- [Preference Page]()
  * Place type choice
  * Skip Button
  * Save Button

- [Home Page]()
  * Plan Today Couresal
    - Plan Today Card
      - Plan Information
        * Plan name
        * Date ( Start - End )
      - `Plan Page`
      - Start Button
      - Close Button
  * Search Bar (Place / User / Plan) - *Call Autocomplete API*
    - `Place Page`
    - `User Page`
    - `Plan Page`
  * Recommended User
    - `User Page`
    - Detail
      - User's name
      - Photo
      - Followers amount
  * Recommended Place
    - `Place Page`
    - Detail
      - Place name
      - Short Location
      - Photo
      - Rating
  * `My Profile Page`
  * `My Plans Page`
  * `Create Plan Page`

- [My Plans Page]()
  * Search Bar (My plan)
  * Plan Card `( Order By Date )`
    * `Plan Page (Custom Plan Button)`
    * Delete Plan Button
    * Status (Planning, Starting, End, Late)
  * `Create Plan Page`

- [Plan Page]()
  * /*Custom Plan Here*/
  * Toggle Button `( Private / Public )`
  * Optimize route
  * Open Google Map Button
  * Plan Information `( Editable )`
    - Title
    - Date
    - Status
    - Setting
      * Plan Type (Autoplan or Selfplan)
      * Level price
  * Day Card `( Order By Date User can choose day to view )`
    - Place card
      * Order Place
      * Photo
      * Name
      * Delete
      * Move to another day
        - To Day
      * Time `( Optional )`
      * (Check Box) `( Disable when not today plan )`
      * `Place Information Page ( Pop up )`
    - Recommended Place Card - *Call Nearby API*
      * Recommended Place Information
        - Photo
        - Name
        - Likes amount
        - Reviews amount
      * `Place Information Page ( Pop up )`
      * Add to plan button

- [Place Information Page]()
  * Place Detail Page
    - Like Button
    - Pinned Button
    - Information
      * Like amount
      * Already Visited
      * Description
      * Photo
      * Rating
      * Level price
      * Open - Close Time
      * Tel `(ดึง Google API, Copy พาไปหน้าโทร)`
    - Share Button
  * Show location on Google Map Button

- [Place Page]()
  * Place Detail Page
    - Like Button
    - Pinned Button
    - Information
      * Like amount
      * Already Visited
      * Description
      * Photo
      * Rating
      * Level price
      * Open - Close Time
      * Tel `(ดึง Google API, Copy พาไปหน้าโทร)`
    - Add to Trip Button
    - Share Button
    - `View Goole Map Page`
    - `Review Place Page (คนยังไม่ไปก็มารีวิวได้)`
      
- [Place Review Page]()
  * Action
    - Report
    - Edit `( Owner Only )`
    - Delete `( Owner Only )`
  * Description
  * Photo
  * Rating
  * Like amount
  - Review user's information
    * Photo
    * Name
    * Badge `( Bronze, Silver, Gold )`

- [Create Plan Page]()
  * /*Choose Main Option for plan Here*/
  * Mandatory setting
    - Source
    - Destination
    - Plan
      * Selfplan `( Default )`
      * Autoplan
  * Optional setting
    - Level price `( Avg. if not select )`
    - Specific type
  * Suggest Existing Plan 
    - Rating
    - Level price `( If choose option )`
    - Specific type `( If choose option )`
  * `Plan Page ( Create Button )`

- [User Page]() /*View Other User Profile*/
  * User's Information
    - Photo
    - FirstName
    - Username
    - Followers amount
    - Reviews amount
    - Badge
  * Place user post
    - Photo
    - Description
  * User's Plan Card
    - Photo
    - Title
    - Number of day
    - `Plan Page ( View only )`
  * `Review Place Page ( View user's review )`


- [My Profile Page]()
  * `User Page ( Editable )`
  * `Edit Profile Page`
  * `Setting Page`

- [Edit Profile Page]()
  * User's Information
    - Photo
    - FirstName
    - LastName
    - Username
    - Email
    - Birthday
    - Addresses
      * Sub district
      * District
      * Province
      * Postal Code
- [Setting Page]()
  * `User's Preference Page`
  * `About us`
  * `Log out`

- [User's Preferences Page]()
  * (Format)
    - (Date format)
    - (Distance format)
    - (Time format)
  * Place type card
    - Name
    - Selected button
# User Function `(User ทำอะไรได้บ้าง)`

- Login
- Register
- Forget Password
- Preference
- Search
- Recommended User
- Recommended Place
- Place Information
- Place Review
- View Profile
- Edit Profile
- Plan List
- Plan Today
- View Plan
- Create Plan
- Edit Plan
- Delete Plan
- Notification

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
- checkbox for place already gone
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
- ระบุเวลาเริ่มต้น - สิ้นสุด (optional)
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

## Notification
- แจ้งเตือนก่อนวันไปเที่ยว 1 วัน
- แจ้งเตือนเมื่อถึงวันไปเที่ยว / เลยวันไปเที่ยว (แต่ยังอยู่ในช่วงไปเที่ยว ให้รีบมาเข้าแอพเราเร็ว)
- แจ้งเตือนเมื่อเลยวันสุดท้าย (คุณอยากทำไรกับแพลนหน่อยมั้ย เข้ามาเลื่อนวันไปเที่ยว)
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
