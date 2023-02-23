<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [three-move-controller](./three-move-controller.md) &gt; [MoveController](./three-move-controller.movecontroller.md) &gt; [tick](./three-move-controller.movecontroller.tick.md)

## MoveController.tick() method

Must be called periodically.

**Signature:**

```typescript
tick(deltaTime: number): void;
```

## Parameters

|  Parameter | Type | Description |
|  --- | --- | --- |
|  deltaTime | number | <code>THREE.Clock.getDelta()</code> |

**Returns:**

void

## Example


```ts
const clock = new THREE.Clock();
renderer.setAnimationLoop(() => {
  const dt = clock.getDelta();
  moveController.tick(dt);
});
```
or

```ts
const clock = new THREE.Clock();
setInterval(() => {
  const dt = clock.getDelta();
  moveController.tick(dt);
}, anything);
```
