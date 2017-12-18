Is the element of unknown height?
=================================

It's still possible to center it by nudging it up half of it's height after bumping it down halfway:

.parent {
  position: relative;
}

.child {
  position: absolute;
  top: 50%;
  transform: translateY(-50%);
}