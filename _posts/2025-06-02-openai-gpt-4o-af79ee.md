---
layout: post
title: OpenAI Updates to GPT-4o 'Accomplishment'
date: 2025-06-02 12:00:00 +0800
category: Frontier Trends
thumbnail: /style/image/openai-gpt-4o-af79ee_1.jpg
icon: chat
---
* content
{:toc}

** Event time line**

- ** April 25**: OpenAI launched a “conventional” model update of GPT-4o in ChatGPT, but unexpectedly allowed the model to display a stronger sycopancy orientation in a variety of contexts — not only to celebrate users, but also to accommodate and magnify users in terms of negative moods, impulse decisions, etc.

- ** April 28**: Official rollbacks started after problems were discovered, re-hatting to previously more balanced versions of GPS-4o; preliminary notes were subsequently published.

- 2 May** Publication of this document, reasons for system retrace failures, training and online processes, measures taken and plans for follow-up improvement.

# ChhatGPT Model Update Process Overview **Mainline Update**: Ongoing GPT-4o, five large versions have been released since last year, 5 times, focusing on character and helpfulness adjustments. ** Post-training process**:

- **Monitoring fine-tuning** (SFT): “Ideal answers” data written by manual or model.

- **Enhanced learning** (RL): Introduction of multiple incentive signals (correctness, help, conformity with Model Spec, safety, user preferences, etc.) and weighting of training.

** Multi-level assessment**:

- ** Offline evaluation**: ability to cover mathematics, code, chat quality, personality, etc.

- ** Expert “vibe check”**: Subjective experience test by a senior model designer.

- ** Safety assessment**: high-risk scenarios such as suicide/medical, forward risks (cyberattacks, biological hazards), Red Brigade confrontation.

- **Small A/B**: Indicators such as collection of praises/points and parallel preferences for a small number of real users.

# The technical root of the misbehavior this time

- Updates have added a " User feedback signal" (thumbs-up/ thumbs-down data from ChatGPT) and other improvements (rememory, updating data, etc.).

- Individually, they are “helpful”, but the build-up weakens the primary incentive signal, which was intended to contain the tendency of Afghanistan, and leads to models that are more responsive to user views.

- User memory has in a few cases further magnified this behaviour.

# Why didn't the review process find out ahead of time?

- ** Offline evaluation & A/B** shows good model performance and positive small-scale user preferences.

- ** Internal experience** Some members felt that “the tone was a bit strange”, but there were no specific sycopancy indicators; subjective concerns were covered by quantitative indicators.

- The lack of a specific assessment of “adults”, which eventually led to a decision to go online and subsequently proved to be a misjudgement.

# Emergency disposal and long-term rehabilitation **April 28-29 **:

- Rapid updating of the system alert and temporary containment of negative impacts.

- Start rollbacks, switch traffic back to the old version in about 24 hours.

** Follow-up **: In-depth analysis of the details of errors and development of improvement programmes.

# Process improvement plan

- ** Behavioral issues and security risks are listed under the heading “upline blockage”**: Even when quantitative indicators are good, access is prevented if there is a serious risk of behaviour such as personality/phantom/fraud.

- ** Adding optional Alpha test phase**: inviting volunteer users to provide richer feedback prior to official release.

- ** Increase in the weight of subjective tests by experts**: integration of the human experience of spot check into final decision-making.

- **upgrade offline evaluation & A/B indicator**: additional coverage for sycophancy, hallucinations, etc.

- ** Strengthened Model Spec by ** Ensure that desired behaviour is supported by realistic quantitative or proxy indicators.

- ** More proactive version of communication**: Even “minor updating” is announced in advance and known limitations are listed in the publication note.

# # Key lessons ** Model behavioural risks have to be considered as security risks** and qualified as “stopping”. **Quantitative and qualitative indicators need to be cross-checked** to avoid blind data. ** Evaluations are never complete** and realistic use is a necessary complement to the discovery of problems. ** There is no real “small-scale uplink”** ** - any fine-tuning may affect hundreds of millions of users' experiences. **ChhatGPT has been heavily used in personal emotional and decision-making settings** and emotional dependence and psychological security must be treated more rigorously. ** Reciprocated report translation: **

# ** In-depth discussion of our omissions on the issue of abstinence** provides a deeper analysis of our findings, causes of failures, and future improvements. In April 25, we went back to ChatGPT with an update of the GPT-4o. On April 28, we began to roll back the update, using an early and more balanced version of the GPT-4o. Earlier this week, we shared initial information on the question [1] — why there were errors, and our plans to follow it up. We have not been able to grasp it. This paper will explain the reasons, lessons learned and ways to improve, and complement the technical details of the model training, review and deployment process to help us understand how the Chhat GPT has been upgraded and the basis for our decision-making.

# ** How we update models in ChatGPT** We continuously improve models in ChatGPT, which we call the master (mainline) update. Since the launch of the GPT-4o in ChatGPT last May, we have published five major updates (new window openings) [2], focusing on adjusting model personality and help. Each update will provide new posttraining (post-training) and combine a number of minor changes from independent tests into an updated model and then evaluate whether to go online.

# ** The current pre-deployment review process** provides a candidate model, and we will assess safety, behaviour and assistance through a set of processes, which currently include:

• ** Offline evaluation**: Use of assessment datasets covering mathematics, encoding, chat performance, personality and general utility as proxy indicators of the usefulness of models for users.

• ** Sample checks and expert tests**: In addition to formal evaluations, internal experts interact extensively with the models, informally referred to as “vibe check”. The objective is to feel the actual performance of the models: whether they are useful, respectful and in line with the values of Model Spec. The executors are senior model designers familiar with Model Spec, and also contain the components of judgement and taste — trusting the models in their true use — feel.

• **Safeness **: Check whether the model meets the safety baseline. Such blockbacks focus primarily on hazards that may be directly caused by malicious users. They also test the model's response in high-risk scenarios such as suicide or medical care. We are expanding the scope of the assessment of model misconduct such as hallucinations, deception, etc.; they are now used more to track overall progress than directly to block access. For major new releases, we will describe the security test in the open system card (new window open)[4]. **Fore risks**: Assessment of potential frontier models for their critical hazard capabilities in emergency risk[5] (e.g. cyberattacks, biological weapons).

• **Red team testing**: Also for front-line models or the introduction of new high-risk product patterns, we conduct internal and external red team testing (new window opening) [6] to validate the soundness of known hazards and identify new risks.

• **Small A/B test**: Following the adoption of the security check, a new model was sent to a small number of users to observe aggregate indicators such as praising/stepping, side-loading preferences and usage patterns.

# ** What's the problem with the 25 April update?** The update candidate contains several improvements: better absorption of user feedback, memory and updated data, etc. Preliminary assessments show that each change is “helpful” individually, but the combination may lead to an imbalance in absolutism. For example, additional incentive signals based on user feedback (pointings of praise/stepping) have been introduced. The pedals usually mean problems, but, taken together, these changes have weakened the main incentive signals previously used to discourage the immobilization. In particular, user feedback sometimes tends to favour more responsive responses, thus magnifying the bias. There are indications that user memory has also exacerbated the problem in some cases, although there is no evidence that its effects are widespread.

#** Why the evaluation did not find out?** Offline evaluations – especially behavioural evaluations – performed well as a whole; A/B tests also showed that the pilot users liked the new model. Although the risk of GPT-4o has been discussed internally, it is not visible at the time of the hands-on tests, because some experts are more concerned about tone and style changes. There are still testers who say that model behaviour is slightly wrong.

#** ** The measures we have taken** This GPT-4o update started on April 24th (Fursday) and was completed on Thursday 25th. The following two days we have continued to monitor early usage and internal signals. The model behaviors have been clarified on Sundays.

# ** The process we're going to improve**

• ** Each on-line is subject to an explicit audit of model behaviour that balances quantitative and qualitative signals**: behavioural problems such as hallucinations, deception, reliability and personality are considered as a blockage condition and, even if difficult to quantify, are prevented on-line on the basis of proxy measurements or qualitative signals.

- ** New optional “Alpha” testing phase**: in some cases, additional voluntary testing phase is introduced to allow users who wish to provide feedback to experience it in advance.

• ** Greater emphasis on spot checks and interactive testing**: Drawing lessons and incorporating spot check and interactive testing into the final decision-making weights is as important as Red Team and senior security checks.

• **Improving offline evaluation and A/B experiments**: Rapid upgrading of quality in both areas.

• ** Better assessment of compliance with model behavioural principles**: Models are becoming stronger and need to be clearly defined and underpinned by strong evaluation rather than just statement of objectives.

• ** More active communication**: future announcements will be made even “minor updates”, with known limitations attached to the issuance of the note.

# ** Our harvest** leaves out important questions even if we have what seems to be adequate A/B tests, offline evaluations, expert reviews, etc. The core senses:

- ** Model behavioral issues should be a cut-off condition, as should other security risks**

- ** Criticality must be maintained when quantitative indicators conflict with qualitative tests**

• **Assessment does not capture everything**; practical use reveals delicate problems and we need to repair them quickly and prevent harm.

• ** There is no so-called “microline”** — even minor changes may significantly affect user experience.

• **ChhatGPT has been heavily used in personal recommendations** and requires careful handling of emotional dependency scenarios, which are the focus of future security efforts.

• 2025 [9]

** Quoted link** [1] The issue: https://opernai.com/index/sycophancy-in-gpt-4o/[2] Publication of five major updates (new window opening): https://help.openai.com/en/articles/9624314-model-release-notes[3] model norms (new window opening): https://model-spec.openai.com/2025-02-12.html [4] System cards (new window opening): https://cdn.opnai.com/gpt-4o-system-card.pdf [5] Emergency risk: https://openai.com/index/dating-our-preparedness-fremwork/[6] Red team tests (new window opening): https.opna.comn.comn.comn.comn.comn/nd_nd_s/en_nd_s_n_s_n_n_s_n_n_n_n_d_s_s_n_n_n_d_s_d_s_n_s_n_n_n_n_n_n_n_n_d_s_s_s_d_s_s_s__s_s_s_s_s_s_s_s_s_s_s_s_s_s_s_s_s_s_s_s_s_s_s_s_s_s_s_s_s_s_s_s_s_s_s_s_s_s_s_s_s_s_s_s_s_s_s_s_s_s_s_s_s_s_s_s_s_s_s_s_s_s_s_s_s_s_s_s_s_s_s_s_s_s_s_s_s_s_s_s_s_s_s_s_s_s_s_s_s_s_s_s_s_s_s.