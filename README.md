# statcast-explorations

## Aim

Apply statistical and machine learning approaches to answer questions about how
MLB batters, pitchers, fielders, and managers make decisions, leveraging the
[Statcast database](https://baseballsavant.mlb.com/statcast_search).

## Investigations

### [Situational Hitting](https://github.com/decohn/statcast-explorations/tree/main/topics/situational-hitting)

Imagine it's the bottom of the 9th inning. The score is tied and there are two
outs, but there's a runner on 3rd. The batter who steps to the plate knows that
a hit - any hit - wins the game. This is the time to shorten up your swing,
forego hitting for power, and just slap the ball past an infielder.

But is boosting batting average at the expense of power something that batters
can actually do on demand? Can batters prioritize hitting the ball to the right
side after a leadoff double, or avoid hitting ground balls when there's a runner
on first and less than two outs?

In other words - is situational hitting real?

* Part One: [Anatomy of a Double Play](https://decohn.github.io/statcast-explorations/topics/situational-hitting/01.anatomy_of_a_double_play.html)
* Part Two: [To Swing or Not to Swing](https://decohn.github.io/statcast-explorations/topics/situational-hitting/02.to_swing_or_not_to_swing.html) (in progress)

### Spray Hitting (planned)

When a batter crushes a line drive directly at an outfielder, it's easy to think
of them as unlucky. If the ball had been hit a couple dozen feet to either side,
it would have easily been a double or a triple into the gap. Statcast metrics
like expected batting average (xBA) try to remove this element of luck found in
traditional statistics by measuring only quality of contact (i.e., launch speed
and launch angle).

But we know that spray angle isn't *entirely* luck. Some batters hit regularly
to all fields, while some are extreme pull hitters. Shouldn't being a
consistent, predictable pull hitter be a disadvantage since it allows for
advantageous defensive positioning? But at the same time, the fences are closer
in left and right field than they are in centre, which favours pull hitters.

Either way, spray angle matters. Is there a way to incorporate it into
statistics like xBA?