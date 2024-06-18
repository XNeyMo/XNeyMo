<p align="center">
  <img src="https://github.com/XNeyMo/XNeyMo/blob/main/assets/banner.png">
</p>

---

<br>
<br>

```js
import React from 'react';
import Knowledge from '../components/Knowledge'

const FrontendDeveloper = () => {
  const userData = {
    name: "Neyan Montes",
    username: "XNeyMo",
    location: "Cartagena de Indias, Colombia",
    web: "https://xneymo.netlify.app",
    technicalKnowledge: {
      frontend: ["AstroBuild", "ReactJS", "React Native", "TailwindCSS", "HTML", "CSS", "JavaScript"],
      backend: ["FastAPI", "Python", "Rust", "NodeJS"],
      database: ["MongoDB", "JSON"]
    }
  };

  return (
    <div>
      <h1>{userData.name}</h1>
      <p>Username: {userData.username}</p>
      <p>Location: {userData.location}</p>
      <p>Web: <a href={userData.web}>{userData.username}'s Website</a></p>

      {Object.keys(userData.technicalKnowledge).map((category, index) => (
        <Knowledge
          key={index}
          title={`${category.charAt(0).toUpperCase()}${category.slice(1)} Technologies`}
          information={userData.technicalKnowledge[category]}
        />
      ))}
    </div>
  );
}

export default FrontendDeveloper;
```

<br>
<br>

<details>
  <summary><b>Contact</b></summary>

  - Website: [XNeyMo](https://xneymo.netlify.app)
  - GitHub: [XNeyMo](https://github.com/XNeyMo)
  - LinkedIn: [Neyan Montes](https://www.linkedin.com/in/neyanmontes/)
  - UpWork: [Neyan Montes](https://www.upwork.com/freelancers/~016725aa35a6808ac8)
  - Telegram: [XNeyMo](https://t.me/xneymo)
  - Email: [Neyan Montes](mailto:xneymodev@gmail.com)
</details>
