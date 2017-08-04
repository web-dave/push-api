# push-api

### Subscribe/Unsubscribe to Web Push

#### /webpush

method POST

payload
```typescript
{
    user: string;
    action: 'subscribe' || 'unsubscribe';
    subscription: {}
}
```
---
### Get all user

#### /users

method GET
---
### Send Message

#### /msg

method POST

payload
```typescript
{
   users: string[];
   msg: {
     msg: {
       title: string;
       message: string;
     }
     icon?: url | base64;
     badge?: url | base64;
     tag?: string;
     data?: url;
   }
}
```
--- 