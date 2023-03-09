# Dmitriy Maslov

### Full stack developer

### **Contacts:**

**Phone:** +7 922 026 4686\
**Telegram:** [@dmtrack](https://t.me/dmtrack)\
**E-mail:** [dmtrack.dev@gmail.com](mailto:dmtrack.dev@gmail.com)\
**GitHub:** [dmtrack](https://github.com/dmtrack)

---

### **About me:**

I've started my career as a sales-manager in steel pipe trade-house of the largest manufacture plant. This work gave me a bunch of experience and soft-skills.
Now i know how to present myself and product, also have no fear talking to unfamiliar people. While working there filled myself not at the right place, so i decided to try change direction.

One of my hobbies was to adjust systems based on very cool and smart zero-code system called [Planfix](www.planfix.com), so i've decided to continue doing it full-time and remote. I've joined one team and worked there like a tech-specialist on company projects. Also i've created my own studio and we were working on our projects and clients.

Remote work as integrator - adjuster gives me extra free time, which I spend learning Frontend Development. I've decided to dive deeper to the development and manage not only zero-code blocks, but full code writing.

I wish my interest to developing, skills and continuous learning will have led me to the success and i will become demanded developer!

---

### **My Skills:**

-   HTML, CSS
-   JavaScript, TypeScript
-   React, Redux&Toolkit
-   NodeJS, Express, MongoDB, PostgreSQL, FireBase, Websockets
-   GitHub
-   Tailwind, Bootstrap, Ant Design, Materialise UI

---

### **Code example:**

```
class UserController {
    registration: RequestHandler = async (req, res, next) => {
        try {
            const errors = validationResult(req);
            if (!errors.isEmpty()) {
                return next(
                    ApiError.badRequest(
                        'Ошибка валидации при регистрации',
                        errors.array()
                    )
                );
            }
            const response = await userService.registration(req);
            res.cookie('refreshToken', response.refreshToken, {
                maxAge: 30 * 24 * 60 * 60 * 1000,
                httpOnly: true,
            });
            response
                .mapRight((user: IUserResponse) => res.status(200).json(user))
                .mapLeft((e: any) => res.status(401).json(e.message));
        } catch (e) {
            next(e);
        }
    }
    }
```

---

### **Courses**

-   Result School
-   August 2022 - Frontend developer
-   October 2022 - extra React course
-   January 2023 - TypeScript course
-   January - March 2023 - iTransition internship

---

### **Languages**

-   English - Upper-intermediate / Advanced
-   Russian - native
