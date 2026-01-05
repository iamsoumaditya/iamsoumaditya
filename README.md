# 👋 Hello, World!

## @Developer

```typescript
import { Injectable } from "@nestjs/common";
import { Developer } from "./interfaces/developer.interface";

@Injectable()
export class DeveloperProfile implements Developer {
  private readonly metadata = {
    name: "Soumaditya Roy",
    role: "Full Stack Developer",
    location: "Kolkata, West Bengal, IN",
    status: "Building amazing things with code 🚀",
  };

  constructor() {
    this.initialize();
  }

  private initialize(): void {
    console.log("Profile loaded successfully ✨");
  }

  getTechStack(): string[] {
    return [
      "Express", "NestJS", "TypeScript", "React", "Next,js", "PostgreSQL", "MongoDB", "Redis", "Docker", "Nginx",
    ];
  }

  getCurrentFocus(): string {
    return "Building scalable backend systems with NestJS";
  }

  getInterests(): string[] {
    return [
      "Microservices Architecture",
      "Data structures & algorithms",
      "System Design",
      "Open Source Contribution",
    ];
  }

  connect(): Record<string, string> {
    return {
      github: "https://github.com/iamsoumaditya",
      linkedin: "https://linkedin.com/in/soumaditya-roy",
      X: "https://x.com/iamsoumaditya",
      email: "iamsoumadityaroy@gmail.com",
    };
  }

  async collaborate(): Promise<string> {
    return "Always open to interesting projects and collaborations! 🤝";
  }
}
```

---

<!-- ## 📊 @Module: Stats

```typescript
@Module({
  providers: [GitHubStats],
  exports: [GitHubStats],
})
export class StatsModule {
  readonly stats = {
    commits: "1,000+",
    pullRequests: "200+",
    issues: "50+",
    stars: "500+",
  };
}
``` -->
## 📊 GitHub Stats

![GitHub Streak](https://streak-stats.demolab.com/?user=iamsoumaditya)





---

## 🛠️ @Controller: Skills

```typescript
@Controller("skills")
export class SkillsController {
  @Get("backend")
  getBackendSkills(): string[] {
    return ["NestJS", "Express", "Fastify", "Appwrite"];
  }

  @Get("frontend")
  getFrontendSkills(): string[] {
    return ["React", "Next.js", "TypeScript", "Tailwind CSS", "Zustand"];
  }

  @Get("devops")
  getDevOpsSkills(): string[] {
    return ["Docker", "GitHub Actions", "Nginx"];
  }

  @Get("databases")
  getDatabases(): string[] {
    return ["PostgreSQL", "MongoDB", "Redis", "MySQL"];
  }
}
```

---

## 🚀 @Pipe: CurrentProjects

```typescript
@Injectable()
export class CurrentProjectsPipe implements PipeTransform {
  transform(projects: any[]): any[] {
    return [
      {
        name: "Dev Who Code",
        description: "A scalable microservices platform",
        tech: [
          "NestJS", "PostgreSQL", "MongoDB", "Redis", "Docker", "Kubernetes", 
        ],
        status: "In Progress 🔨",
      },
    ];
  }
}
```

---

## 📫 @Gateway: Contact

```typescript
@WebSocketGateway()
export class ContactGateway {
  @SubscribeMessage("connect")
  handleConnection(client: Socket): void {
    const contactInfo = {
      email: "iamsoumadityaroy@gmail.com",
      linkedin: "soumaditya-roy",
      X: "@iamsoumaditya",
      //   portfolio: "https://coming.soon",
    };

    client.emit("contact_info", contactInfo);
  }
}
```

**Let's build something amazing together!** Feel free to reach out for collaborations or just a friendly chat about tech. 💬

---

## 📈 @Interceptor: ActivityLog

```typescript
@Injectable()
export class ActivityInterceptor implements NestInterceptor {
  intercept(context: ExecutionContext, next: CallHandler): Observable<any> {
    const recentActivity = [
      "🎯 Optimized application performance",
      //   "🔥 Contributed to open source",
      //   "💡 Learned new design patterns",
      //   "🐛 Fixed critical bugs",
      //   "📚 Wrote technical documentation",
    ];

    return next.handle();
  }
}
```

---

<div align="center">

### 💭 Developer Quote

```typescript
const philosophyService = {
  getQuote: () => "Code is like humor. When you have to explain it, it's bad.",
};
```

**⭐ Star my repositories if you find them useful!**

![Profile Views](https://komarev.com/ghpvc/?username=iamsoumaditya&color=blueviolet)

</div>
