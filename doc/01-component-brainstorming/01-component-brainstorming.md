# Portfolio Part 1: Component Brainstorming

- **Name**: Hanse Musaogullari
- **Dot Number**: Musaogullari.2

## Pre-Assignment

I am interested in fashion and enjoy finding inspiration from various sources. My goal is to create a project that reflects my passion for creativity and organization while showcasing my skills in software design. The idea of developing something similar to Pinterest excites me because it allows me to combine my love for aesthetics and functionality into a platform that inspires others.

### Component Designs

> Please use this section to share your designs.

- Component Design #1: Board
  - **Description**:

    A Board component represents a collection of content. Users can group items by theme or category, such as fashion trends or inspirational quotes.

  - **Kernel Methods**:

void addItem(Item item)
void removeItem(Item item)
List<Item> getItems()

  - **Secondary Methods**:

   void shareBoard(User user)
   List<Board> searchBoards(String keyword)

  - **Additional Considerations** (*note*: "I don't know" is an acceptable
    answer for each of the following questions):
    - Would this component be mutable? Answer and explain:

      Yes, users can add or remove items, altering the board.

    - Would this component rely on any internal classes (e.g., `Map.Pair`)?
      Answer and explain:

      Maybe, an Item class for individual pins.

    - Would this component need any enums or constants (e.g.,
      `Program.Instruction`)? Answer and explain:

      Yes, for attributes like PUBLIC or PRIVATE visibility settings.

    - Can you implement your secondary methods using your kernel methods?
      Answer, explain, and give at least one example:

      Yes, for example, searchBoards can filter items added to the board.


- Component Design #2: Pins
  - **Description**:

A Pin component represents individual items saved on boards. This could include fashion ideas, images, or links to websites.

  - **Kernel Methods**:

void setDescription(String description):
void setLink(String link)
String getDescription()
String getLink()

  - **Secondary Methods**:

boolean isTrending()
List<Pin> getSimilarPins()

  - **Additional Considerations** (*note*: "I don't know" is an acceptable
    answer for each of the following questions):
    - Would this component be mutable? Answer and explain:

Yes, users can edit the pin's data.

    - Would this component rely on any internal classes (e.g., `Map.Pair`)?
      Answer and explain:

No, unless for data like tags.

    - Would this component need any enums or constants (e.g.,
      `Program.Instruction`)? Answer and explain:

I'm not sure.

    - Can you implement your secondary methods using your kernel methods?
      Answer, explain, and give at least one example:

Yes, isTrending could rely on data about saves or views.

- Component Design #3: User
  - **Description**:

A User component models a person using the platform. It manages their boards, pins, and interactions with other users.

  - **Kernel Methods**:

void createBoard(Board board)
void deleteBoard(Board board)
List<Board> getBoards()

  - **Secondary Methods**:

void followUser(User user)
List<Pin> getSavedPins()

  - **Additional Considerations** (*note*: "I don't know" is an acceptable
    answer for each of the following questions):
    - Would this component be mutable? Answer and explain:

Yes, since users can update their boards and connections.

    - Would this component rely on any internal classes (e.g., `Map.Pair`)?
      Answer and explain:

I'm not sure.

    - Would this component need any enums or constants (e.g.,
      `Program.Instruction`)? Answer and explain:

Possibly, for roles like ADMIN or MEMBER

    - Can you implement your secondary methods using your kernel methods?
      Answer, explain, and give at least one example:

Yes, getSavedPins could cover the boards to compile a list of pins.

## Post-Assignment

The following sections detail everything that you should do once you've
completed the assignment.


You may notice that things are nicely linked in the root CHANGELOG. If you'd
like to accomplish that, you will need to make GitHub releases after each pull
request merge (or at least tag your commits). This is not required.

In the future, the CHANGELOG will be used to document changes in your
designs, so we can gauge your progress. Please keep it updated at each stage
of development.



| Criteria of Constructive Feedback | Missing                                                                                                                           | Developing                                                                                                                                                                                                                                | Meeting                                                                                                                                                               |
| --------------------------------- | --------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Specific                          | All feedback is general (not specific)                                                                                            | Some (but not all) feedback is specific and some examples may be provided.                                                                                                                                                                | All feedback is specific, with examples provided where possible                                                                                                       |
| Actionable                        | None of the feedback provides actionable items or suggestions for improvement                                                     | Some feedback provides suggestions for improvement, while some do not                                                                                                                                                                     | All (or nearly all) feedback is actionable; most criticisms are followed by suggestions for improvement                                                               |
| Prioritized                       | Feedback provides only major or minor concerns, but not both. Major and minar concerns are not labeled or feedback is unorganized | Feedback provides both major and minor concerns, but it is not clear which is which and/or the feedback is not as well organized as it could be                                                                                           | Feedback clearly labels major and minor concerns. Feedback is organized in a way that allows the reader to easily understand which points to prioritize in a revision |
| Balanced                          | Feedback describes either strengths or areas of improvement, but not both                                                         | Feedback describes both strengths and areas for improvement, but it is more heavily weighted towards one or the other, and/or descusses both but does not clearly identify which part of the feedback is a strength/area for improvement  | Feedback provides balanced discussion of the document's strengths and areas for improvement. It is clear which piece of feedback is which                             |
| Tactful                           | Overall tone and language are not appropriate (e.g., not considerate, could be interpreted as personal criticism or attack)       | Overall feedback tone and language are general positive, tactul, and non-threatening, but one or more feedback comments could be interpretted as not tactful and/or feedback leans toward personal criticism, not focused on the document | Feedback tone and language are positive, tactful, and non-threatening. Feedback addesses the document, not the writer                                                 |
