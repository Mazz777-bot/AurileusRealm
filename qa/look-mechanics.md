# Goldsmiths Lion look mechanics

The lion remains grounded on all four paws with the lower torso and paw baseline anchored. Attention is led by the amber eyes, followed by a restrained head-and-neck turn or pitch. The muzzle, nose, eyelids, ears, and mane participate together so each direction reads at normal pet size without stretching the skull or rotating the whole sprite.

The crown is rigidly worn and follows the head with only a tiny physically plausible lag; it never floats or changes design. The centered neck medallion stays attached to the collar and may swing subtly opposite the head motion. Foreleg bracers stay locked to the legs. Mane volume and facial proportions remain constant.

Motion budget: every 22.5-degree step changes eye aim, muzzle direction, head pitch/yaw, ear angle, and near/far mane visibility by a similar small amount. Paws, baseline, body scale, and lower-body registration do not jump. No whole-sprite rotation, affine tilt, replacement eyes, new props, scenery, shadows, text, or detached effects.

## Cardinal pose families

- 000 up: nose lifts above head center, pupils and eyelids aim upward, chin and lower mane become slightly more visible, ears perk; crown tips back with the head while remaining seated.
- 090 screen-right: nose tip and pupils move clearly to the image's right of head center; the lion's rightward face surface becomes the leading side, the opposite cheek and mane recede, and the right-side ear/mane contour leads.
- 180 down: muzzle dips and nose sits below head center, pupils aim downward, upper eyelids lower, crown tips slightly forward, and the collar/medallion remain visible beneath the mane.
- 270 screen-left: nose tip and pupils move clearly to the image's left of head center; the leftward face surface becomes the leading side, the opposite cheek and mane recede, and the left-side ear/mane contour leads.

Diagonals interpolate continuously between adjacent cardinal families. The 157.5-to-180 and 337.5-to-000 boundaries must be exactly one restrained step, with no scale pop, recentering, side flip, or jewelry jump.
