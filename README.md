const Agents = [
  {
    data_collection: {
      agent_details: { firstName: "Alice", lastName: "Mike", id: 1 },
      vulnerability_groups: [
        { firstName: "Mary", lastName: "Jack", vulnerability_group: "Widow", age: 50, id: 1 },
        { firstName: "AudioData", lastName: "Dam", age: 12, vulnerability_group: "Orphan", id: 2 }
      ]
    }
  },
  {
    data_collection: {
      agent_details: { firstName: "Bob", lastName: "Dylan", id: 2 },
      vulnerability_groups: [
        { firstName: "Yilo", lastName: "Joe", vulnerability_group: "Orphan", age: 5, id: 4 },
        { firstName: "Audio", lastName: "Lam", age: 10, vulnerability_group: "Orphan", id: 3 },
        { firstName: "Aud", lastName: "Bob", age: 81, vulnerability_group: "Widow", id: 5 }
      ]
    }
  },
  {
    data_collection: {
      agent_details: { firstName: "Charlie", lastName: "Brown", id: 3 },
      vulnerability_groups: [
        { firstName: "Yilo", lastName: "Joe", vulnerability_group: "Orphan", age: 5, id: 6 },
        { firstName: "Audio", lastName: "Lam", age: 45, vulnerability_group: "Widow", id: 7 },
        { firstName: "Aud", lastName: "Bob", age: 81, vulnerability_group: "Widow", id: 8 }
      ]
    }
  }
];

console.log(Agents);
