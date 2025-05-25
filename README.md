```typescript

export class Dujuniorrr {
    role = 'Web Developer';

    greetingTitle = 'Hello everyone!';

    aboutMe = `I am a web developer with a passion for programming and designing systems with clean and modular architectures. I enjoy being involved in all stages of software engineering during a project — from requirements elicitation, modeling, and planning to development, testing, and deployment.`;

    mainStack: Technology[] = [
        { name: 'PHP', category: 'language' },
        { name: 'Laravel', category: 'framework' },
        { name: 'JavaScript', category: 'language' },
        { name: 'Vue.js', category: 'frontend' },
        { name: 'MySQL', category: 'database' },
        { name: 'Docker', category: 'devops' }
    ];

    otherTechnologies: Technology[] = [
        { name: 'TypeScript', category: 'language' },
        { name: 'Node.js', category: 'backend' },
        { name: 'Python', category: 'language' },
        { name: 'Django', category: 'framework' },
        { name: 'Java', category: 'language' },
        { name: 'Spring', category: 'framework' },
        { name: 'PostgreSQL', category: 'database' },
        { name: 'MongoDB', category: 'database' }
    ];

    getPresentationData(): PresentationData {
        return {
            role: this.role,
            greeting: this.greetingTitle,
            about: this.aboutMe,
            mainStack: this.mainStack,
            otherTechnologies: this.otherTechnologies
        };
    }
}

type Technology = {
    name: string;
    category: 'ambient' | 'database' | 'devops' | 'language' | 'framework' | 'tool';
};

type PresentationData = {
    role: string;
    greeting: string;
    about: string;
    mainStack: Technology[];
    otherTechnologies: Technology[];
}

```
