If you don't know the width or height, you can use the transform property and a negative translate of 50% in both directions (it is based on the current width/height of the element) to center:

.parent {
  position: relative;
}

.child {
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
}