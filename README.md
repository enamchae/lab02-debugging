# lab02-debugging
1. Daniel Chen
2. https://www.shadertoy.com/view/tfsfDf
3. bugs:
   1. type and variable name typo at `vec uv`, needs to be `vec2 uv2`
   2. pass `uv2` to `raycast` instead of `uv` to use [-1, 1] coords
   3. divide by `iResolution.y` instead of `iResolution.x` to fix aspect ratio
   4. adjust number of ray march iterations from 64 to 512 to avoid the floor being clipped
   5. pass `dir` as first arg to `reflect` instead of `eye`

# Setup 

Create a [Shadertoy account](https://www.shadertoy.com/). Either fork this shadertoy, or create a new shadertoy and copy the code from the [Debugging Puzzle](https://www.shadertoy.com/view/flGfRc).

Let's practice debugging! We have a broken shader. It should produce output that looks like this:
[Unbelievably beautiful shader](https://user-images.githubusercontent.com/1758825/200729570-8e10a37a-345d-4aff-8eff-6baf54a32a40.webm)

It don't do that. Correct THREE of the FIVE bugs that are messing up the output. You are STRONGLY ENCOURAGED to work with a partner and pair program to force you to talk about your debugging thought process out loud.

Extra credit if you can find all FIVE bugs.

# Submission
- Create a pull request to this repository
- In the README, include the names of both your team members
- In the README, create a link to your shader toy solution with the bugs corrected
- In the README, describe each bug you found and include a sentence about HOW you found it.
- Make sure all three of your shadertoys are set to UNLISTED or PUBLIC (so we can see them!)
