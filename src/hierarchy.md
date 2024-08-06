```js
// App.tsx

<QueryClientProvider>
  <AppProvider>
    <AppRouter />
  </AppProvider>
</QueryClientProvider>
```

```tsx
// <AppRouter />
{
  isAuthorised ? (
    <MasterLayout>
      <PrivateRoutes />
    </MasterLayout>
  ) : (
    <PublicRoutes />
  )
}
```
