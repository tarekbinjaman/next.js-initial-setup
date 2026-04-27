# Follwoing this steps we can start a next.js project easily here we go

1. Run this:
~~~
npx create-next-app@latest my-frontend
~~~

2. It will ask questions → choose like this:
~~~
✔ TypeScript? → Yes
✔ ESLint? → Yes
✔ Tailwind CSS? → Yes
✔ App Router? → Yes (IMPORTANT)
✔ src/ directory? → Yes
✔ Import alias? → Yes
~~~

3. Then: 
~~~
cd my-frontend
~~~
Then enter  "code ." in cmd

Now, you will see your very first next.js files here

4. open:
npm run dev
[http://localhost:3000](http://localhost:3000)

5. Understand Next.js Structure (Very Important)
Inside src/app:

~~~
app/
 ├── layout.tsx   ← global layout
 ├── page.tsx     ← home page (/)
~~~

👉 In Next.js:
- page.tsx = route
- Folder name = URL

Example:

~~~
app/about/page.tsx → /about
~~~


5. Clean Setup (Recommended)

Delete everything inside page.tsx and write:

~~~
export default function Home() {
  return (
    <div>
      <h1>Hello Tarek 👋</h1>
    </div>
  );
}
~~~