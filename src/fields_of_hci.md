# Forschungsgebiete von HCI
Ein wichtiger Bestand von HCI ist der Mensch selbst. Der Mensch kann in abstrakter Weise mit dem Model Human Processor Modell beschrieben werden.

## Human Processor Model
Das Human Processor Model besagt, dass ein Nutzer die Sinneseindrücke mithilfe eines **Perceptual Processors** verarbeitet und diese dann in zwei unterschiedliche "Speicher" ablegt.
Zum einen gibt es den **Visual Image Store**, in welchem Dinge abgespeichert werden, welche wir **sehen**. Zum Anderen gibt es den **Auditory Image Store**, in welchem Dinge abgespeichert werden, welche wir **hören**.
Diese zwei Speicher sind Bereiche des "Working Memory". Mit genug Übung etc. gehen diese in das "Long Term Memory" über.
Zudem besteht eine Verbindung zum "Motor Processor" und zum "Cognitive Processor".

```mermaid
flowchart LR
    subgraph long_term_memory[Long Term Memory]
    subgraph working_memory[Working Memory]
    visual_image_store[Visual Image Store]
    auditory_image_store[Auditory Image Store]
    end
    end
    motor_processor-->muscles[Muscles]
    working_memory-->motor_processor[Motor Processor]
    long_term_memory-->cognitive_processor
    cognitive_processor[Cognitive Processor]<-->working_memory
    perceptual_processor[Perceptual Processor]-->visual_image_store & auditory_image_store
    senses[Senses]-->perceptual_processor
```
*Human Processor Model*

## Seven Stages of Action
Die Seven Stages of Action beschäftigen sich primär mit *drei Hauptfragen**:
* Wie kann man den Nutzer dabei unterstützen, die nächste Interaktion zu **planen**?
* Wie kann man den Nutzer dabei unterstützen, die nächste Interatktion **auszuführen**?.
* Wie kann man den Nutzer dabei unterstützen, den Zustand des Systems **richtig wahrzunehmen**?

## Seven Stages of Action
```mermaid
flowchart TB
   goals[Goals]
   subgraph plan[Planen]
   intention_to_act[Intention to act]
   sequence_of_action[Sequence of action aka plan]
   end
   subgraph execute[Ausführen]
   execution_of_action[Execution of the action]
   end
   subgraph perceive[Wahrnehmen]
   perceiving_the_state[Perceiving the state of the world]
   interpreting_the_perception[Interpreting the perception]
   evaluating_the_interpretations[Evaluating the interpretations]
   end
   goals-->intention_to_act-->sequence_of_action-->execution_of_action-->perceiving_the_state-->interpreting_the_perception-->evaluating_the_interpretations
   evaluating_the_interpretations-->goals
```
 *Seven Stages of Action*