# ECAsT
Expanded-CAsT: A multi-turn conversation paraphrase dataset.

Expanded-CAsT (ECAsT) is a multi-turn paraphrase dataset built using TREC CAsT conversations. There are currently very few datasets available for training and evaluating conversational search systems, and ECAsT aims to address this limitation by augmenting the original dataset with paraphrased turns.

ECAsT is built using the first three years of CAsT releases (2019, 2020, and 2021). The dataset expands the size of the original CAsT collection by over 665\%, resulting in a total of 9,214 turns across 131 open-domain topics. This substantial increase in data volume can significantly benefit the development and evaluation of conversational search systems.

## Dataset Fields
The dataset comprises three columns:
* __Turn_ID:__ The first column contains the turn identifier, which is a combination of the conversation topic ID and turn ID, separated by an underscore. All turns with the same topic ID belong to the same conversation, and the turn ID indicates the depth of the question within the conversation. Rows with identical turn_IDs are paraphrases of each other, and the turn_IDs correspond to the original TREC CAsT conversations that were paraphrased.
* __Raw Paraphrase:__ Raw paraphrases represent conversation turns with omissions and co-references. These turns reflect how a user would naturally ask the system for information within a conversation.
* __Manual Paraphrase:__ Manual paraphrases denote conversation turns that fully express the user's information need. These turns depict how a user would pose the question as a standalone query, without relying on conversation context.

## Statistics
By paraphrasing the CAsT dataset, ECAsT expands it by over 665\%, resulting in a new dataset consisting of 9,214 turns over 131 conversation topics. On average, there are 7.6 paraphrases per original CAsT turn.
