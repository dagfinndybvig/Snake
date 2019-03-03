# Snake
Borrowed this from tayloraliss for practice. 
He followed tutorial from "LibGDX Game Development by Example" by James Cook.
I added accelerometer controls so it can be played on Android.

The code I added (starting from ||) to the queryInput() part of the render-method of GameScene was basically:

        boolean aPressed = (Gdx.input.isKeyPressed(Input.Keys.Z)) || (Gdx.input.getAccelerometerX()>2);
        boolean dPressed = (Gdx.input.isKeyPressed(Input.Keys.X)) || (Gdx.input.getAccelerometerX()<-2);
        boolean wPressed = (Gdx.input.isKeyPressed(Input.Keys.K)) || (Gdx.input.getAccelerometerY()<-2);
        boolean sPressed = (Gdx.input.isKeyPressed(Input.Keys.M)) || (Gdx.input.getAccelerometerY()>2);
