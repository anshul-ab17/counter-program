#counter-program::rust!


</br>

next_account_info: Fn for nxt account from the i/p acc
AccountInfo: Struct  represents what an i/p account wants
entrypoint!: macro that marks the program's entry
msg!: logs runtime.
ProgramResult: result type by Solana programs.
 
</br>


program_id  deployed program
</br>

accounts: &[AccountInfo], // An array of input addresses. This array should have all the addresses the user is going to interact with when they are calling this function.
</br>

instruction_data- array of bytes, but it can be deserialized into a struct,contains information/ instruction

</br>
acc -Gets the first account in the list. This is expected to be the account holding the Counter
</br>
instruction_type- Deserialize the incoming instruction bytes into an InstructionType.
</br>
counter_data -Reads and deserializes the Counter struct from the account data.