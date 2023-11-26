Intent Filters




What are the three criteria an acticity’s intent filter must fulfill in order for a system to send an intent to that activity?

In order for a system to send an intent to an activity, the activity must fulfill three criteria in its intent filter:

Action (Required): The action is a string that specifies the general action to be performed. It's a mandatory field and defines what the component does. Examples include "ACTION_SEND" for sending data and "ACTION_VIEW" for viewing data.

Data (Optional): This field specifies the data type and URI format that the component can handle. It's optional, but if included, the system will check whether the incoming data matches the specified criteria.

Category (Optional): Categories further describe the activity. They are optional but can help in refining the types of components that can respond to an intent.

How does an activity retrieve the Intent that it was started by?




an activity retrieves the intent that started it by calling the getIntent() method. This method returns the Intent object that was used to launch the activity. The activity can then extract any data or information passed in the intent.

Explain intents to a non-technical friend.




, think of intents as messages your smart assistant (phone) understands. When you ask it to do something, like open a photo, you're sending a message (intent) that tells your phone what you want. The phone then figures out which part (like the photo viewer) should handle it, making your request happen seamlessly. It's like giving instructions to your assistant, and your phone takes care of the details to make things happen.













Implicit vs. Explicit Intents

Compare and contrast implicit and explicit intents.

Explicit Intents:

Purpose: Explicit intents specify a particular component within your own application that should respond to the intent. You use them when you know the target component's class name or package name.

Use Case: Typically used when you want to initiate an action within your own app, such as starting a new activity or invoking a service.




Implicit Intents:

Purpose: Implicit intents don't specify a particular component but declare a general action to be performed. They allow components from other apps to respond to the intent based on their capabilities.

Use Case: Used when you want to delegate a task to another app that can handle it, without specifying the exact app. For instance, if you want to show a location on a map, you can use an implicit intent, and any map app installed on the device can respond.




What is the primary information contained within an Intent?

Component name

Action

Data

Category

Extras

Flags


