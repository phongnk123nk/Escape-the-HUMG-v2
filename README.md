# Escape The HUMG

## 1. Hướng dẫn tải dự án về máy

Làm theo các bước sau:

1. Mở link dự án trên GitHub:

```text
https://github.com/phongnk123nk/Escape-the-HUMG-v2
```

2. Bấm nút **Code** màu xanh.

3. Chọn **Download ZIP**.

4. Chờ file ZIP tải xong.

5. Giải nén file ZIP ra một thư mục dễ tìm trên máy, ví dụ:

```text
D:\UnityProjects\Escape-the-HUMG-v2
```

6. Sau khi giải nén, mở thư mục đó ra và kiểm tra có các thư mục sau:

```text
Assets
Packages
ProjectSettings
```

Nếu có đủ 3 thư mục trên thì đã tải đúng dự án Unity.

Không mở trực tiếp project trong file ZIP. Phải giải nén ra trước.

## 2. Hướng dẫn tải Unity Hub

Unity Hub là phần mềm dùng để cài Unity và mở project Unity.

Làm theo các bước sau:

1. Mở trang tải Unity:

```text
https://unity.com/download
```

2. Bấm **Download for Windows** hoặc **Download Unity Hub**.

3. Chờ file cài đặt tải xong.

4. Mở file vừa tải về và cài Unity Hub.

5. Cài xong thì mở **Unity Hub**.

Nếu Unity yêu cầu đăng nhập, hãy đăng nhập bằng tài khoản Unity hoặc tạo tài khoản miễn phí.

## 3. Add project vào Unity Hub và mở project

Sau khi đã có Unity Hub, tiến hành thêm project vừa tải về vào Unity Hub.

### Hình 1: Bấm Add và chọn Add project from disk

![Hình 1: Add project from disk](docs/images/hinh-1-add-project-from-disk.png)

Trong Unity Hub:

1. Vào tab **Projects**.
2. Bấm nút **Add**.
3. Chọn **Add project from disk**.

### Hình 2: Chọn thư mục vừa giải nén

![Hình 2: Chọn thư mục vừa giải nén](docs/images/hinh-2-chon-thu-muc-giai-nen.png)

Ở cửa sổ chọn thư mục:

1. Tìm đến nơi đã giải nén project.
2. Chọn thư mục có tên gần giống:

```text
Escape-the-HUMG-v2-main
```

3. Bấm **Open**.

Lưu ý: chọn thư mục project, không chọn riêng thư mục `Assets`.

### Hình 3: Chọn project Escape The HUMG để mở

![Hình 3: Chọn project Escape The HUMG để mở](docs/images/hinh-3-chon-project-escape.png)

Sau khi add xong, Unity Hub sẽ hiện project trong danh sách.

1. Tìm project có tên **Escape-the-HUMG-v2-main** hoặc tên bắt đầu bằng **Escape The HUMG**.
2. Kiểm tra cột **Editor version** là Unity `6000.3.9f1` hoặc gần đúng bản đó.
3. Bấm vào tên project để mở.

Lần đầu mở sẽ hơi lâu vì Unity phải import lại toàn bộ asset.

Lưu ý: Khi mở project, Unity Hub thường sẽ tự đề xuất phiên bản Unity phù hợp với dự án. Chỉ cần làm theo đề xuất đó để cài/mở đúng phiên bản. Lần đầu bật game lên có thể mất thời gian khá lâu vì Unity phải tải package, import asset và tạo lại dữ liệu project.

### Hình 4: Vào Assets > Scenes và chọn scene cần xem

![Hình 4: Chọn scene trong Assets Scenes](docs/images/hinh-4-chon-scene.png)

Sau khi Unity mở project:

1. Nhìn xuống cửa sổ **Project** ở phía dưới.
2. Vào thư mục:

```text
Assets
```

3. Mở tiếp thư mục:

```text
Scenes
```

4. Chọn scene muốn xem hoặc muốn chạy.

Scene nên mở đầu tiên là:

```text
main menu.unity
```

Sau khi mở scene, bấm nút **Play** ở phía trên Unity để chạy game.

Ghi chú nhanh về các scene chính:

```text
main menu.unity          Màn hình menu chính của game
room1.unity              Màn/phòng đầu tiên sau menu
hanh lang 1.unity        Khu vực hành lang 1
hanh lang 2.unity        Khu vực hành lang 2
hanh lang 3.unity        Khu vực hành lang 3
PhongThiNghiem.unity     Phòng thí nghiệm
PhongTinHoc.unity        Phòng tin học
BangXepHinh.unity        Màn xếp hình
GOODENDING.unity         Màn good ending
ending 1.unity           Màn ending khác
ESC.unity                Màn/menu ESC
```

Ghi chú vị trí các script/code trong project:

```text
Assets/                         Các script chính của game
Assets/Scripts/                 Script phụ, hiện có EndingCutscene.cs
Assets/Editor/                  Script chỉ dùng trong Unity Editor để setup scene
Assets/ChessKnightImported/Scripts/   Script mini-game quân mã
Assets/DeliveryCarImported/Scenes/    Script mini-game giao hàng/xe
Assets/ESC/Scripts/             Script menu ESC/pause
Assets/image/Animation/         Script animation mũi tên
Assets/scr logo1/               Script màn xếp hình/logo
```

Một số script quan trọng:

```text
Assets/MainMenuButtonActions.cs                  Nút ở menu chính
Assets/HallwayImageNavigator.cs                  Điều hướng hành lang
Assets/HallwayArrowHotspot.cs                    Vùng bấm/mũi tên hành lang
Assets/ComputerRoomNavigator.cs                  Logic phòng tin học
Assets/ComputerRoomHotspot.cs                    Vùng tương tác phòng tin học
Assets/LabSceneNavigator.cs                      Logic phòng thí nghiệm
Assets/LabInventorySystem.cs                     Hệ thống kéo/thả đồ
Assets/LabEquationPuzzleManager.cs               Câu đố phương trình
Assets/RoomIntroVideoPlayer.cs                   Video intro room1
Assets/GlobalEscPauseMenu.cs                     Menu tạm dừng
Assets/ChessKnightImported/Scripts/GameManager.cs     Quản lý mini-game quân mã
Assets/ChessKnightImported/Scripts/BoardManager.cs    Bàn chơi mini-game quân mã
Assets/DeliveryOrderMiniGameManager.cs           Quản lý mini-game giao hàng
Assets/scr logo1/QuanLyXepHinh.cs                Quản lý màn xếp hình/logo
```
