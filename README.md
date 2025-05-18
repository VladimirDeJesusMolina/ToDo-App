# Todo App with Next.js 14, MongoDB & Prisma

<img width="1436" alt="Screenshot 2025-05-18 at 7 22 32 PM" src="https://github.com/user-attachments/assets/ffdcc649-f7c5-4aff-959f-93c68727daf7" />


A full-stack Todo application built by following https://www.youtube.com/watch?v=9OoKXOq7ENo

## ✨ Features
- **Full CRUD Operations**
  - ✅ Create new todos
  - ✏️ Edit existing todos
  - 🗑️ Delete todos
  - ✅ Toggle completion status
- **Modern Stack**
  - Next.js 14 (App Router)
  - Prisma ORM
  - MongoDB Atlas
  - TypeScript
- **Optimistic UI Updates**
- **Responsive Design**

## 🛠️ What I Learned
Through building this project, I implemented:

1. **Next.js Setup**
   - App Router configuration
   - Server Actions for data mutations

2. **Prisma Integration**
   - MongoDB schema definition
   - Prisma Client initialization

3. **Core Functionality**
   ```typescript
   // Example Server Action
   async function createTodo(formData: FormData) {
     'use server'
     await prisma.todo.create({
       data: { title: formData.get('title') }
     })
   }
