<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
    <style>
        ::placeholder{color: black}
        h2{color: blue; text-align: center;}
        .mytextbox{
            color: black; background-color: #46d6de;
            border: 1px solid #288ba3; width: 300px;
            text-shadow: 2px 2px 3px white}
        .mytextbox:hover{font-weight: bolder;}
        #form1 table { border: 5px groove #993366;
            background-color: #FFCCCC;color: #0539a0;}
        #form1 table td {border: 1px solid #CC9999;}
    </style>
</head>
<body>
    <h2>ĐĂNG KÝ THÀNH VIÊN CLB YÊU NHẠC</h2>
    <FORM  id="form1" method="post" enctype="multipart/form-data" action="XuLyDangKy.php">
        <table align="center" border="1" style="border-radius: 5%;">
        <tr>
            <td>Họ tên</td>
            <td>
                <input class="mytextbox" type="text" name="txtHoTen" required 
                placeholder="Vui lòng nhập họ tên" />
            </td>
        </tr>
        <tr>
            <td>Độ tuối trung bình</td>
            <td>
                <input class="mytextbox" type="number" min="18" max="45" value="20">
            </td>
        </tr>
        <tr>
            <td>Thành phố</td>
            <td>
                <select class="mytextbox" name="thanhpho">
                    <option value="ct">Cần Thơ</option>
                    <option value="sg">TPHCM</option>
                    <option value="hn">Hà Nội</option>
                    <option value="bd">Bình Dương</option>
                    <option value="bp">Bình Phước</option>
                    <option value="cm">Cà Mau</option>
                </select>
            </td>
        </tr>
        <tr>
            <td>Tên đăng nhập</td>
            <td>
                <input class="mytextbox" name="txtUserName" required />
            </td>
        </tr>
        <tr>
            <td>Mật khẩu</td>
            <td>
                <input class="mytextbox" type="password" name="txtPass" required 
                placeholder="Mật khẩu" />
            </td>
        </tr>
        <tr>
            <td>Gõ lại mật khẩu</td>
            <td>
                <input class="mytextbox" type="password" name="txtRepass" required 
                placeholder="Mật khẩu" />
            </td>
        </tr>
        <tr>
            <td>Phái</td>
            <td>
                <input  type="radio" name="rdPhai" value="0" checked>Nam
                <input type="radio" name="rdPhai" value="1" >Nữ 
            </td>
        </tr>
        <tr>
            <td>Ngoại ngữ</td>
            <td>
                <input type="checkbox" name="chkAnh" value="0" >Anh
                <input type="checkbox" name="chkPhap" value="1" >Pháp
                <input type="checkbox" name="chkHoa" value="2" >Hoa
            </td>
        </tr>
        <tr>
            <td>Nghề nghiệp</td>
            <td>
                <select class="mytextbox" name="cboNgheNghiep">
                    <option value="0">Bạn làm nghề gì</option>
                    <option value="1">Học sinh - Sinh viên</option>
                    <option value="2">Giáo viên</option>
                    <option value="3">Bác sĩ</option>
                    <option value="4">Kỹ sư</option>
                </select>
            </td>
        </tr>
        <tr>
            <td>Hình</td>
            <td>
                <input class="mytextbox" type="text">
                <input type="file" name="fHinh">
            </td>
        </tr>
        <tr>
            <td>Sở thích</td>
            <td>
                <textarea class="mytextbox" name="txtSoThich" id="" cols="30" rows="10"></textarea>
            </td>
        </tr>
        <tr>
            <td colspan="2" Align="center">
                <button style="background-color: aquamarine;" name="btnDangKy">Đăng ký</button>
                <button style="background-color: aquamarine;"name="btnXoa">Làm lại</button>
                <input hidden name="Ngaydangky" value="16/09/2023">
            </td>
            <td></td>
        </tr>
        </table>
    </FORM>
</body>
</html>
