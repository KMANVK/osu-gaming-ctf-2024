# Challenge 1 : forensics/nathan-on-osu

## Des : Here's an old screenshot of chat logs between sahuang and Nathan on hollow's Windows machine, but a crucial part of the conversation seems to be cropped out... Can you help to recover the flag from the future?

## Sol : Sử dụng các công cụ như Acropalypse để khôi phục hình ảnh với độ phân giải phù hợp. => https://acropalypse.app/ 

![image](https://github.com/KMANVK/osu-gaming-ctf-2024/assets/94669750/4a665cc0-13f0-44eb-9eac-c260f5d818b9)

## Flag : `osu{cr0pp3d_Future_Candy<3}`

# Challenge 2 : forensics/volatile-map 

## Des : Hey osu! players, our SOC team was informed that a group of spies from Mai Corp is trying to sabotage our infrastructure via their secret map in osu!. We were able to break into their rendezvous, but they noticed we were stealing their data and they corrupted them in time. Fortunately, we managed to acquire a full memory dump from one of their machines. Can you help us investigate what they were trying to do?

## Sol : Chúng ta được cung cấp một kho lưu trữ bộ nhớ để điều tra. Vì vậy, bằng cách sử dụng vol3 với plugin pslist, tôi đã tìm được chương trình osu!.exe chạy các phiên bản notepad.exe. 

![image](https://github.com/KMANVK/osu-gaming-ctf-2024/assets/94669750/99dc18fa-b792-4b0b-bda2-9066f4101cfa)

![image](https://github.com/KMANVK/osu-gaming-ctf-2024/assets/94669750/77f1be82-286e-48b8-aa70-2023f979a6ab)

+ Check process `note.exe` bằng cmdline :

![image](https://github.com/KMANVK/osu-gaming-ctf-2024/assets/94669750/76e5de30-bcb3-4a22-8855-d92259258d8b)

# Challenge 3 : out-of-click

## Des : I love playing this map but recently I noticed that some of the circles seem off. Can you help me find the locations of the weird circles?

## Sol : Chúng ta được cung cấp một thư mục beatmap. Nhìn vào đó, có các loại beatmap khác nhau (Normal, Out of Click, Time Freeze). Đọc câu hỏi, tôi giả định rằng sự khác biệt có thể được tìm thấy bằng cách so sánh Mormal và out of Click của beatmap.

![image](https://github.com/KMANVK/osu-gaming-ctf-2024/assets/94669750/ef9e1986-7c91-40c6-b709-2d5b5c67bc2e)

+ So sánh 2 file bằng tool : https://www.diffchecker.com/text-compare/

+ Sau khi so sánh ta nhận được các giá trị decimal lần lượt :

![image](https://github.com/KMANVK/osu-gaming-ctf-2024/assets/94669750/446798bd-9287-4a68-9580-8ac0c8c2d78c)

![image](https://github.com/KMANVK/osu-gaming-ctf-2024/assets/94669750/5adb5a5f-899a-4d77-a83b-37bd1ecece83)

![image](https://github.com/KMANVK/osu-gaming-ctf-2024/assets/94669750/e7175de4-f3da-4de0-a097-bcbbb48f6dd4)

![image](https://github.com/KMANVK/osu-gaming-ctf-2024/assets/94669750/f289e721-608c-41b7-913a-26bb749eaabc)

![image](https://github.com/KMANVK/osu-gaming-ctf-2024/assets/94669750/5da7050d-7459-4c07-8681-daf1b411ee03)


=> `111, 115, 117, 123, 66, 84, 77, 67, 95, 49, 53, 95, 109, 89, 95, 71, 48, 97, 84, 125`

![image](https://github.com/KMANVK/osu-gaming-ctf-2024/assets/94669750/8dec327a-13f7-4215-9352-5552053253cf)






