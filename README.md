## Setup
```
npx create-next-app@latest next-discord --typescript --tailwind --eslint
npx shadcn-ui@latest init
```

## Feature
- [Clerk Auth](https://clerk.com/)
- [Next-Theme](https://ui.shadcn.com/docs/dark-mode/next)
- query-string
- [Livekit](https://livekit.io/)
- socket.io : real time chat
- useContext
- @emoji-mart/react & @emoji-mart/data :Emoji picker
- @tanstack/react-query : pagination update
- Primsa & [PlanetScale](https://planetscale.com) && Mysql : Database


npx prisma migrte reset

prisma
deleteMany:{
	id:xxxx
}

## Additional Notes
1. Copy Paste Method
navigator.clipboard.writeText(inviteUrl);

2. Key down event
const down = (e: KeyboardEvent) => {
if (e.key === "k" && (e.metaKey || e.ctrlKey)) {
    e.preventDefault();
    setOpen((open) => !open);
   }
}

document.addEventListener("keydown", down);

3. Reset Prisma migration
```
npx prisma migrte reset
```

4. Paginatio Loading
[Check out](https://github.com/tenPro4/next_discord23/blob/main/hooks/use-chat-query.ts)
