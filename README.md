# SGC.Update

Kênh thông báo cập nhật cho các addin BIMUP. Addin đọc file này mỗi lần mở phần mềm.

`revit.txt`:
- Dòng 1: version mới nhất (so với AssemblyVersion của DLL)
- Dòng 2: link tải bản cài
- Dòng 3+: ghi chú cập nhật

URL addin đọc: `https://raw.githubusercontent.com/KsPhong/SGC.Update/main/revit.txt`

## Phát hành bản mới
1. Tăng `AssemblyVersion` trong BIMUP.Revit, build bản cài.
2. `gh release create revit-v1.3.0 BIMUP-Revit-1.3.0.msi -R KsPhong/SGC.Update`
3. Sửa `revit.txt` (version + link tải), commit, push.
