## Pitch Location & Movement

px → x-location as pitch crosses the plate (X=0 means right down the middle).

pz → z-location as pitch crosses the plate (Z=0 means the ground).

pfx_x → Horizontal movement relative to a straight-line path (in inches).

pfx_z → Vertical movement relative to a straight-line path (in inches).


## Pitch Speed & Spin

start_speed → Speed of the pitch just as it's thrown. (MPH?)

end_speed → Speed of the pitch when it reaches the plate. (MPH?)

spin_rate → The pitch's spin rate, measured in RPM (Revolutions Per Minute).

spin_dir → Direction in which the pitch is spinning, measured in degrees.


## Pitch Break & Acceleration

break_angle → The angle at which the pitch breaks (measured in degrees).

break_length → The total distance the pitch moves due to breaking action (in inches).

break_y → The point along the y-axis where the pitch starts to break.

ax → Acceleration of the ball in the x-direction (ft/s²).

ay → Acceleration of the ball in the y-direction (ft/s²).

az → Acceleration of the ball in the z-direction (ft/s²).


## Strike Zone Boundaries

sz_bot → Bottom of the batter’s strike zone (in feet).

sz_top → Top of the batter’s strike zone (in feet).


## Pitch Classification & Confidence

type_confidence → Confidence in pitch classification (sometimes goes up to 2).

pitch_type → Type of pitch (e.g., FF = Four-Seam Fastball, SL = Slider).


## Velocity Components (Initial Conditions of the Pitch)

vx0 → Initial velocity of the pitch in the x-direction (ft/s).

vy0 → Initial velocity of the pitch in the y-direction (ft/s).

vz0 → Initial velocity of the pitch in the z-direction (ft/s).

x0 → Initial x-position of the pitch at release (ft).

y0 → Initial y-position of the pitch at release (ft).

z0 → Initial z-position of the pitch at release (ft).


## Game Context & Results

x → x-location of the pitch at the plate (similar to px).

nasty → A score representing how difficult the pitch was to hit (higher = harder).

zone → The strike zone region the pitch crossed (based on MLB zones).

### Zones 1-9 Represent the area within the strike zone, encompassing the area over home plate between the batter's knees and the midpoint between their shoulders and the top of their uniform pants.

### Zones 11-14 These zones represent pitches outside the strike zone, considered balls.

### code → Records the result of the pitch (see dataset description for code meanings).

### type → Simplified pitch result:

"S" = Strike

"B" = Ball

"X" = In-play event (hit, out, etc.).


## Game and At-Bat Information

event_num → Event number (useful for identifying game sequences like ejections).

b_score → Batter’s team score at the time of the pitch.

ab_id → At-bat ID (links with atbats.csv).

b_count → Number of balls in the current count.

s_count → Number of strikes in the current count.

outs → Number of outs (before pitch is thrown).

pitch_num → Pitch number within the current at-bat.


## Base Runners (On-Base Situation)

on_1b → True if a runner is on first base, False if it is empty.

on_2b → True if a runner is on second base, False if it is empty.

on_3b → True is a runner is on third base, False if it is empty.
