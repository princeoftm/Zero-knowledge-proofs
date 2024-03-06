Personally Identifiable Information (PII) shared with third-party services is stored in central databases, which are vulnerable to hacks. With identity theft becoming a critical issue, there are calls for more privacy-protecting means of sharing sensitive information.



Zero-knowledge proofs solve this problem by eliminating the need to reveal information to prove validity of claims. The zero-knowledge protocol uses the statement (called a ‘witness’) as input to generate a succinct proof of its validity. This proof provides strong guarantees that a statement is true without exposing the information used in creating it.

How do zero-knowledge proofs work?
A zero-knowledge proof allows you to prove the truth of a statement without sharing the statement’s contents or revealing how you discovered the truth. To make this possible, zero-knowledge protocols rely on algorithms that take some data as input and return ‘true’ or ‘false’ as output.

A zero-knowledge protocol must satisfy the following criteria:
```
Completeness: If the input is valid, the zero-knowledge protocol always returns ‘true’. Hence, if the underlying statement is true, and the prover and verifier act honestly, the proof can be accepted.
```
```
Soundness: If the input is invalid, it is theoretically impossible to fool the zero-knowledge protocol to return ‘true’. Hence, a lying prover cannot trick an honest verifier into believing an invalid statement is valid (except with a tiny margin of probability).
```
```
Zero-knowledge: The verifier learns nothing about a statement beyond its validity or falsity (they have “zero knowledge” of the statement). This requirement also prevents the verifier from deriving the original input (the statement’s contents) from the proof.
```


In basic form, a zero-knowledge proof is made up of three elements: witness, challenge, and response.

```
Witness: With a zero-knowledge proof, the prover wants to prove knowledge of some hidden information. The secret information is the “witness” to the proof, and the prover's assumed knowledge of the witness establishes a set of questions that can only be answered by a party with knowledge of the information. Thus, the prover starts the proving process by randomly choosing a question, calculating the answer, and sending it to the verifier.
```
```
Challenge: The verifier randomly picks another question from the set and asks the prover to answer it.
```
```
Response: The prover accepts the question, calculates the answer, and returns it to the verifier. The prover’s response allows the verifier to check if the former really has access to the witness. To ensure the prover isn’t guessing blindly and getting the correct answers by chance, the verifier picks more questions to ask. By repeating this interaction many times, the possibility of the prover faking knowledge of the witness drops significantly until the verifier is satisfied.
```