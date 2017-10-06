# public_data

For use in personal projects.

## ICOW Data
217 observations of countries across 15 variables:

1. __State:__ COW Country Code
*  The COW country code for the state.
2. __Name__: Name of State
*  The state's name (in some cases I have changed this from the original COW name for purposes of precision or clarification).
3. __ColRuler__: Primary Colonial Ruler
*  The colonial or imperial power that was most responsible for shaping the development of the entity (or entities) that became this modern state. This is typically the state that ruled over the majority of this territory (for cases where multiple colonial powers held parts of what became the modern state) or the state that ruled over this territory for the longest time (for cases where the colony changed hands one or more times before independence).
*  Note that this may not be the state from which this entity received its independence, which is covered by a separate set of variables in the data set. For example, although the UK and France took possession of Ottoman territories in the Middle East as League of Nations mandated territories after World War I, the states that resulted are coded as having been part of the Ottoman Empire.
4. __IndFrom__: Entity from Which Independence Was Gained
* The COW country code for the state, empire, or other entity from which this state gained independence. This variable is coded as missing where the state did not gain independence from a COW system member (e.g., by unifying local units into a new state).
5. __IndDate__: Date of Independence
* The date on which this state became independent -- i.e., acquired control of its own foreign policy, without being ruled by a foreign power. This takes the form YYYYMM, where the month is coded as 00 if ICOW does not currently have an estimated month when the state took its current form.
* Note that unlike the Polity 2 and COW Territorial Change data sets, which are left-censored in 1800 and 1816 respectively, this data set does not left-censor dates of independence. Dates before 1800 or 1816 are coded as relevant; this applies primarily to the European powers, as well as to a few older states in other regions.
6. __IndViol__: Violent Independence?
* 1: Yes = The independence occurred through organized violence.
* 0: No = The independence did not involve organized violence.
* An independence process is considered violent if it occurred through armed revolt by the entity, or if it occurred through armed conflict between the former ruler and another state (as when the entity in question is conquered or freed by a foreign power, or when it changed hands as part of a treaty ending a war).
7. __IndType__: Type of Independence
* 1: Formation = The entity was formed from other entities that have no direct analog in the COW interstate system. (For example, the United Kingdom became independent without seceding from or being colonized by the equivalent of any current COW actors)
* 2: Decolonization = The entity was a dependency ruled by a foreign power before achieving independence. (Note that this includes traditional colonies, protectorates, and parts of empires, as well as any other entities that were ruled by a foreign power or that were part of an entity that was not in the COW system.)
* 3: Secession = The entity was part of another state before achieving independence, with the original state surviving in reduced form. (Note that seceding from a colonial empire or other entity that isn't part of the COW interstate should be coded as decolonization; secession only refers to leaving a COW system member that remains in the system afterward, as with Eritrea leaving Ethiopia, or with most of the former republics leaving the Soviet Union or Yugoslavia while Russia or Serbia remained.)
* 4: Partition = The entity was partitioned out of another state as it achieved independence, with the original state not surviving. (Note that seceding from a colonial empire or other entity that isn't part of the COW interstate should be coded as decolonization; partition only refers to leaving a COW system member that does not remain in the system afterward, as with the former Czechoslovakia.)
* • This is adapted from a typology used by the COW Territorial Change data set, excluding some types of changes that are not relevant to independence (such as conquest or peaceful cession).
8. __SecFrom__: Entity from Which State Seceded
* • The COW country code for the state from which this state seceded after independence. This variable is coded as missing where the state did not secede from a COW system member.
* • Note that secession means that this state was an integral part of the state from which secession occurred; this is different from decolonization, where the new state was ruled as a colony or other dependency of the state from which independence was achieved.
9. __SecDate__: Date of Secession
* • The date on which this state seceded. This takes the form YYYYMM, where the month is coded as 00 if ICOW does not currently have an estimated month when the state took its current form.
10. __SecViol__: Violent Secession?
* 1: Yes = The secession occurred through organized violence.
* 0 : No = The secession did not involve organized violence.
* • A secession process is considered violent if it occurred through armed revolt by the entity, or if it occurred through armed conflict between the former ruler and another state (as when the entity in question is conquered or freed by a foreign power, or when it changed hands as part of a treaty ending a war).
11. __Into__: Entity into which State Merged
* • The COW country code for a state that absorbed this state after independence. This variable is coded as missing where the state did not merge into a COW system member.
12. __IntoDate__: Date of Merger into Other Entity
* • The date on which this state merged into the other entity. This takes the form YYYYMM, where the month is coded as 00 if ICOW does not currently have an estimated month when the state took its current form.
13. __COWsys__: COW Interstate System Entry
* • The date on which this state entered the COW interstate system (according to system list 2004.1).
14. __GWsys__: Gleditsch & Ward System Entry
* • The date on which this state entered the Gleditsch & Ward interstate system (obtained from Kristian Gleditsch's web site, as updated through the end of 2002).
15. __Notes__: Notes about Colonial History or Independence
* • This section includes notes about different codings from different data sets, as well as brief interruptions in system membership that do not justify coding a new independence afterward.
