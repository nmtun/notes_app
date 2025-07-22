# Notes App 📝

Một ứng dụng quản lý ghi chú đơn giản và hiệu quả được xây dựng với React.js (Frontend) và Node.js/Express (Backend).

## 🌟 Demo
🔗 **Live Demo**: [Notes App](https://notes-app-2ilc.vercel.app/)

## ✨ Tính năng

- 🔐 **Xác thực người dùng**: Đăng ký, đăng nhập an toàn với JWT
- 📝 **Quản lý ghi chú**: Tạo, chỉnh sửa, xóa ghi chú
- 🏷️ **Tag hệ thống**: Phân loại ghi chú bằng tags
- 🔍 **Tìm kiếm**: Tìm kiếm ghi chú theo tiêu đề và nội dung
- 📌 **Ghim ghi chú**: Đánh dấu ghi chú quan trọng
- 🤖 **Chatbot trò chuyện thân thiện**: Hỗ trợ người dùng 24/7
- 📱 **Responsive**: Tối ưu cho mọi thiết bị
- 🎨 **UI hiện đại**: Giao diện đẹp mắt với Tailwind CSS

## 🛠️ Công nghệ sử dụng

### Frontend
- **React.js** - Thư viện UI
- **Vite** - Build tool
- **Tailwind CSS** - Framework CSS
- **React Router** - Navigation
- **Axios** - HTTP client
- **React Icons** - Icon library
- **React Modal** - Modal components
- **Moment.js** - Date formatting

### Backend
- **Node.js** - Runtime environment
- **Express.js** - Web framework
- **MongoDB** - Database
- **Mongoose** - ODM
- **JWT** - Authentication
- **bcrypt** - Password hashing
- **CORS** - Cross-origin resource sharing
- **Cloudinary** - Image storage (nếu có)

## 📁 Cấu trúc Project

```
notes_app/
├── frontend/           # React.js frontend
│   ├── src/
│   │   ├── components/    # Reusable components
│   │   ├── pages/        # Page components
│   │   ├── utils/        # Utility functions
│   │   └── assets/       # Static assets
│   ├── index.html
│   └── package.json
│
├── backend/            # Node.js backend
│   ├── models/         # Database models
│   ├── config.json     # Database configuration
│   ├── index.js        # Main server file
│   ├── utilities.js    # Utility functions
│   └── package.json
│
└── README.md
```

## 🚀 Cài đặt và Chạy

### Yêu cầu hệ thống
- Node.js (v14 hoặc cao hơn)
- npm hoặc yarn
- MongoDB

### 1. Clone repository
```bash
git clone https://github.com/nmtun/notes_app.git
cd notes_app
```

### 2. Cài đặt Backend
```bash
cd backend
npm install
```

### 3. Cấu hình Database
Tạo file `config.json` trong thư mục backend:
```json
{
  "connectionString": "mongodb://localhost:27017/notes-app"
}
```

### 4. Chạy Backend
```bash
npm start
```
Backend sẽ chạy trên `http://localhost:8000`

### 5. Cài đặt Frontend
```bash
cd ../frontend
npm install
```

### 6. Chạy Frontend
```bash
npm run dev
```
Frontend sẽ chạy trên `http://localhost:5173`

## 🔧 Cấu hình Environment Variables

### Backend (.env)
```env
ACCESS_TOKEN_SECRET=your_jwt_secret_key
CLOUDINARY_CLOUD_NAME=your_cloudinary_name
CLOUDINARY_API_KEY=your_api_key
CLOUDINARY_API_SECRET=your_api_secret
```

## 📖 API Endpoints

### Authentication
- `POST /create-account` - Tạo tài khoản mới
- `POST /login` - Đăng nhập

### Notes
- `GET /get-all-notes` - Lấy tất cả ghi chú
- `POST /add-note` - Tạo ghi chú mới
- `PUT /edit-note/:noteId` - Chỉnh sửa ghi chú
- `DELETE /delete-note/:noteId` - Xóa ghi chú
- `PUT /update-note-pinned/:noteId` - Ghim/bỏ ghim ghi chú
- `GET /search-notes/` - Tìm kiếm ghi chú

### User
- `GET /get-user` - Lấy thông tin người dùng

## 🎯 Hướng dẫn sử dụng

1. **Đăng ký tài khoản** mới hoặc **đăng nhập** nếu đã có tài khoản
2. **Tạo ghi chú mới** bằng cách click nút "Add Note"
3. **Thêm tags** để phân loại ghi chú
4. **Ghim ghi chú** quan trọng để dễ tìm kiếm
5. **Tìm kiếm** ghi chú bằng thanh search
6. **Chỉnh sửa/Xóa** ghi chú khi cần thiết

## 🚀 Deployment

### Frontend (Vercel)
1. Push code lên GitHub
2. Kết nối với Vercel
3. Deploy tự động

### Backend (Vercel)
1. Tạo file `vercel.json` với cấu hình phù hợp
2. Deploy qua Vercel CLI hoặc GitHub integration

## 🤝 Đóng góp

1. Fork repository
2. Tạo feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to branch (`git push origin feature/AmazingFeature`)
5. Tạo Pull Request

## 📝 License

Distributed under the MIT License. See `LICENSE` for more information.

## 👨‍💻 Tác giả

**nmtun** - [GitHub Profile](https://github.com/nmtun)

## 🙏 Acknowledgments

- React.js team
- Express.js team
- MongoDB team
- Tailwind CSS team
- Vercel for hosting

---

⭐ Nếu project này hữu ích, hãy give một star nhé! ⭐